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

<style scoped>
    .subscribe-section{
        background-color: #E56768;
        margin-top: 45px;
    }

    .row{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .subscribe-title{
        color: white;
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
        background: #E9D758;
        border-radius: 50%;
        color: white;
        font-size: 20px;
    }

    .button-subscribe:hover{
        background-color: #E56768;
    }
</style>