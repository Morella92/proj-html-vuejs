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

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .hero-section{
        background-color: rgba(224, 112, 114, 0.9);
        position: relative;
        color: $tertiary;
        text-align: center;
        overflow: hidden;
    }

    .hero-section::before{
        content: "";
        display: block;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-image: url('../../public/img/theme_slider2_bg-1.jpg');
        background-size: cover;
        opacity: 0.1;
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
        background-color:$secondary;
        color: $tertiary;
        margin-right: 36px;
    }

    .courses-button:hover{
        background-color: $tertiary;
        color: $bg-primary;
    }
    .apply-button{
        color: $bg-primary;
    }

    .apply-button:hover{
        background-color: $secondary;
        color: $tertiary;
    }

    .hero-wave{
        margin: -5px;
    }
</style>