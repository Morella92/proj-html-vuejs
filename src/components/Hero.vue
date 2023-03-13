<script>
    export default {

    }
</script>

<template>
    <section class="hero-section">
        <div class="container">
            <h1 class="hero-title">Key to your success</h1>
            <p class="hero-p">
                EduPrime is the most versatile WordPress theme for educational purposes, <br>
                showcase universities, courses, secondary schools, etc.
            </p>

            <button class="courses-button">
                <i class="fa-solid fa-magnifying-glass"></i>
                Search courses
            </button>

            <button class="apply-button">
                <i class="fa-solid fa-user-plus"></i>
                Apply for university
            </button>
        </div>
        <img class="hero-wave" src="../../public/img/Wave-1.png" alt="">
    </section>

</template>

<style scoped>
    .hero-section{
        background-color: #DE6E70;
        /* background-image: url('../../public/img/theme_slider2_bg-1.jpg');
        background-size: cover;
        filter: grayscale(100%) brightness(100%); */
        color: white;
        text-align: center;
    }

    .hero-title{
        font-size: 48px;
        margin-bottom: 48px;
    }

    .hero-p{
        font-size: 18px;
        line-height: 20px;
    }

    .courses-button, .apply-button{
        padding: 21px 41px;
        font-size: 15px;
        border-radius: 50px;
        font-weight: 600;
        margin-top: 50px;
        margin-bottom: 118px;
    }

    .courses-button{
        background-color:#E9D758;
        color: white;
        margin-right: 36px;
    }

    .apply-button{
        color: #DE6E70;
    }

    .hero-wave{
        margin: -5px;
    }
</style>