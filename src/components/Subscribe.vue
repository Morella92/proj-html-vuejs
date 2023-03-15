<script>
    export default {

    }
</script>

<template>

    <section class="subscribe-section">
        <div class="container-small">
            <div class="row">
                <div class="col">
                    <h2 class="subscribe-title">Subscribe Now to Our Newsletter!</h2>
                </div>
                <div class="col">
                    <input class="email-input" type="email" placeholder="Email address...">
                    <button class="button-subscribe"> <i class="fa-solid fa-paper-plane"></i></button>
                </div>
            </div>
            
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .subscribe-section{
        background-color: $bg-primary;
        margin-top: 45px;
    }

    .row{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .subscribe-title{
        color: $tertiary;
        font-size: 35px;
        font-weight: 600;
        padding: 43px 0;
    }

    .email-input{
        border-radius: 35px;
        height: 70px;
        font-size: 15px;
        border: 0;
        padding: 25px;
        width: 500px;
        position: relative;
    }

    .button-subscribe{
        position: absolute;
        right: 73px;
        height: 70px;
        padding: 21px 28px;
        background: $secondary;
        border-radius: 50%;
        color: $tertiary;
        font-size: 20px;
    }

    .button-subscribe:hover{
        background-color: $bg-primary;
    }

    @media screen and (max-width: 991px) {
        .button-subscribe{
            right: 20px;
        }

        .col{
            padding: 0 20px;
        }
    }

    @media screen and (max-width: 767px){
        .row{
            flex-direction: column;
        }

        .button-subscribe{
            right: 130px;
        }

        .col{
            margin-bottom: 20px;
        }
    }
</style>