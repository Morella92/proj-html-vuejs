<script>
    export default {
        data(){
            return{

                eduPrime:[
                    'Request a Website',
                    'Browse Themes',
                    'Payment Option',
                    'Support System',
                    'Checkout',
                    'Purchase Theme'
                ],

                networking:[
                    'Purchase Theme',
                    'Our Benefits',
                    'Our Team',
                    'Our Services',
                    'Other Products',
                    'My account'
                ],

                buttons:[
                    'Economy',
                    'Design',
                    'Coaching',
                    'Business',
                    'Medicine',
                    'Law',
                    'Fitness'
                ]
            }
        }
    }
</script>

<template>
    <section class="footer-section">
        <div class="container-small">
            <div class="row-footer">
                <div class="col">
                    <img class="logo" src="../../public/img/theme_eduprime_logo.png" alt="">
                    <p class="footer-p">
                        Eduprime is the most versatile WordPress theme for <br> educational purposes,
                        showcasing universities, <br> courses, secondary schools, etc.
                    </p>
                    <div>
                       <span class="footer-icons"><i class="fa-brands fa-facebook-f"></i></span>
                       <span class="footer-icons"><i class="fa-brands fa-twitter"></i></span> 
                       <span class="footer-icons"><i class="fa-brands fa-instagram"></i></span> 
                    </div>
                </div>
                <div class="col">
                    <h3 class="footer-titles">Get Eduprime</h3>
                    <ul v-for="list in eduPrime">
                        <li class="list-items">
                            {{ list }}
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h3 class="footer-titles">Networking</h3>
                    <ul v-for="network in networking">
                        <li class="list-items">
                            {{ network }}
                        </li>
                    </ul>
                </div>
                <div class="col col-info">
                    <div class="searchbar">
                        <input class="search-input" type="text" placeholder="Search...">
                        <button class="button-footer"> <i class="fa-solid fa-magnifying-glass"></i></button>
                    </div>
                    <h4 class="search-title">Search Categories</h4>
                    <ul class="buttons">
                        <li v-for="button in buttons">
                            <button class="button-style">
                                {{button}}
                            </button>
                        </li>
                    </ul>
                    <h5 class="privacy">ModelTheme.All rights Reserved.</h5>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .footer-section{
        background-color: $bg-primary;
        color: $tertiary;
        margin-top: -4px;
    }

    .row-footer{
        padding-top: 86px;
        padding-bottom: 65px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 10px;
    }

    .col{
        flex-basis: calc(100% / 4);
    }
    .logo{
        width: 250px;
    }

    .footer-p{
        padding: 20px 0;
        font-size: 16px;
    }

    .footer-icons{
        border: 2px solid $secondary;
        border-radius: 50%;
        padding: 10px 15px;
        width: 50px;
        height: 50px;
        font-size: 18px;
        margin: 0 5px;
    }

    .footer-icons:hover{
        background-color: $secondary;
    }
    .footer-titles{
        margin-bottom: 18px;
        font-size: 20px;
    }

    .list-items{
        font-size: 16px;
        line-height: 28px;
    }

    .list-items:hover{
        color: $secondary;
    }
    .search-input{
        border-radius: 35px;
        height: 70px;
        font-size: 15px;
        border: 0;
        padding: 25px;
        width: 300px;
        position: relative;
        margin-bottom: 20px;
    }

    .button-footer{
        position: absolute;
        right: 70px;
        height: 70px;
        padding: 21px 28px;
        background: $secondary;
        border-radius: 50%;
        color: $tertiary;
        font-size: 20px;
    }

    .button-footer:hover{
        background-color: $bg-primary;
    }

    .col-info{
        display: flex;
        flex-direction: column;
        align-items: flex-end;
    }

    .buttons{
        display: flex;
        flex-wrap: wrap;
        gap: 7px;
        margin: 15px 0;
    }

    .button-style{
        background-color: $bg-primary;
        color: $tertiary;
        border: 1px solid $tertiary;
        border-radius: 50px;
        font-size: 12px;
        text-transform: uppercase;
        padding: 6px 15px;
    }

    .button-style:hover{
        background-color: $secondary;
    }
    .privacy{
        color: $secondary;
        font-size: 16px;
        font-weight: 300;
    }
</style>