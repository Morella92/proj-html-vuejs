<script>
    export default {
        data(){

            return{

                navItem: [
                    'Home',
                    'Courses',
                    'About Us',
                    'News',
                    'Pages',
                    'Contact',
                    'Purchase'
                ],
            }
        },
    }
</script>

<template>

    <section class="navbar-section">
        <div class="container flex-rules">
            <div class="logo">
                <img src="../../public/img/theme_eduprime_logo.png" alt="">
            </div>

            <ul class="list-flex">
                <li v-for="item in navItem" :key="item" class="nav-list-style">
                    <a href="#" class="margin-rule">{{ item }}</a>
                    <i class="fa-solid fa-caret-down" v-if="['Home', 'Courses', 'News', 'Pages'].includes(item)"></i>
                </li>
            </ul>

            <button class="nav-button">
                View Courses
            </button>

            <div class="menu-icon">
                <i class="fa-solid fa-bars"></i>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .navbar-section{
        background-color: rgba(224, 112, 114, 0.9);
    }

    .flex-rules{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .logo{
        width: 290px;
    }

    .list-flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 33px;
    }
    
    .nav-list-style{
        font-size: 17px;
        color: $tertiary;
        font-weight: 600;
    }

    .nav-list-style:hover{
        color: $secondary;
    }

    .margin-rule{
        margin-right: 12px;
    }
    .nav-button{
        color: $tertiary;
        background-color: $secondary;
        border-radius: 50px;
        padding: 15px 35px;
        font-size: 17px;
        font-weight: 600;
        text-transform: uppercase;
        line-height: 33px;
    }

    .nav-button:hover{
        background-color: $tertiary;
        color: $bg-primary;
    }

    .menu-icon{
        font-size: 40px;
        border: 2px solid black;
        padding: 5px 10px;
        background-color: $tertiary;
        display: none;
    }

    @media screen and (max-width: 991px) {
        .flex-rules {
            flex-direction: column;
            align-items: center;
        }

        .logo {
            margin-top: 20px;
        }

        .list-flex {
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-button {
            margin-top: 20px;
        }
    }

    @media screen and (max-width:767px){

        .navbar-section{
            background-color: #3D404F;
        }
        .list-flex, .nav-button{
            display: none;
        }

        .menu-icon{
            display: block;
        }

        .flex-rules{
            flex-direction: row;
        }
    }
</style>