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
                ]
            }
        }
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
        </div>
    </section>

</template>

<style>
    .navbar-section{
        background-color: #DE6E70;
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
        font-size: 14px;
        color: white;
        font-weight: 600;
    }

    .margin-rule{
        margin-right: 12px;
    }
    .nav-button{
        color: white;
        background-color:#E9D758;
        border-radius: 50px;
        padding: 10px 25px;
        font-size: 14px;
        font-weight: 600;
        text-transform: uppercase;
        line-height: 33px;
    }
</style>