<script>
    export default {
        data(){
            return{

                facultyName:[
                    'Law faculty',
                    'Economy',
                    'Medicine',
                    'Computer Science',
                    'Graphic Design'
                ],

                facultyImage: [
                    '../../public/img/Gavel-v2.png',
                    '../../public/img/Coins-tabs-v2.png',
                    '../../public/img/Medicine-tabs-v2.png',
                    '../../public/img/Computer-tabs-v2.png',
                    '../../public/img/Palette-tabs-v2.png'
                ]
            }
        }
    }
</script>

<template>
    <section class="faculty-section">
        <div class="container-small">
            <div class="row">
                <div class="col-courses">
                    <img class="book-img" src="../../public/img/Books-icon.png" alt="">
                    <h2 class="courses-title">Thousands of courses <br> for any type of students</h2>
                    <p class="courses-p">
                        At EduPrime, it doesn’t matter what domain you wish to pursue a career in. 
                        Here you <br> can find a course that satisfies your needs within a click away and applies for a 
                        course <br> in a matter of minutes. EduPrime is ranked as the most versatile university in the world, <br>
                        thanks to the number of courses it provides.
                    </p>
                    <button class="courses-button">Browse through courses</button>
                </div>
                <div class="col-hat">
                    <img class="hat-img" src="../../public/img/Graduation-Illustration.png" alt="">
                    <!-- <img class="hat-bg" src="../../public/img/home-background.png" alt=""> -->
                </div>
            </div>

            <div class="faculty-choice">
                <h2 class="courses-title">Faculties available at EduPrime</h2>
                <p class="courses-p"> 
                    A single university with a load of courses, tailored <br>
                    to satisfy any student’s needs.
                </p>
            </div>
            
            
            <ul class="row shadow">
                <li v-for="(name, index) in facultyName" :key="index" 
                :class="name === 'Law faculty' ? 'faculty-list-pink' : ''" class="faculty-list">
                    <a href="#">
                        <img :src="facultyImage[index]" class="faculty-images">
                        <h4 class="faculty-name">{{ name }}</h4>
                    </a>
                </li>
            </ul>

            <div class="law-faculty">
                <div class="row">
                    <div class="col">
                        <img class="law-image" src="../../public/img/Gavel-Illustration-e1556884768193.png" alt="">
                    </div>
                    <div class="col">
                        <h2 class="courses-title">Law Faculty</h2>
                        <p class="courses-p">
                            Learning from world-leading academics and practitioners, you’ll not only receive an outstanding grounding in the theory of law, but you will be able to understand how those principles are applied in practice through a range of student-led activities and competitions.
                        </p>

                        <button class="law-button">Read more</button>
                    </div>
                </div>
            </div>
        </div>
        
        <img class="wave-bottom" src="../../public/svg/svg-0.svg" alt="">
    </section>
</template>

<style scoped>
    .row{
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .col-courses, .law-faculty{
        margin-top: 100px;
        margin-bottom: 50px;
    }
    .book-img{
        width: 68px;
        margin-bottom: 20px;
    }
    .courses-title{
        font-size: 48px;
        color: #3d404f;
        line-height: 56px;
    }

    .courses-p{
        font-size: 16px;
        color: #3D404F;
        line-height: 30px;
        margin: 40px 0;
        margin-right: 40px;
    }

    .courses-button{
        background-color: #e9d758;
        color: white;
        font-weight: 600;
        font-size: 17px;
        padding: 23px 45px;
        border-radius: 50px;
    }

    .courses-button:hover{
        background-color: #DD3333;
    }

    .hat-img{
        width: 470px;
        /* background-image: url('../../public/img/home-background.png'); */
    }

    .faculty-choice{
        text-align: center;
        margin-top: 145px;
    }

    .shadow{
        box-shadow: 10px 10px 5px #dedede;
    }
    .faculty-list{
        border: 0.5px solid #EAEAEA;
    }

    /* .faculty-list-pink{
        filter: hue-rotate(0deg);
        background-color: #E56768;
    } */
    .faculty-images{
        width: 95px;
        margin: 35px 68px;
    }

    .faculty-name{
        text-align: center;
        color: #E56768;
        font-size: 17px;
        font-weight: 600;
        margin-bottom: 10px;
    }

    .law-image{
        width: 330px;
        margin: 0 110px;
    }

    .law-button{
        background-color: #E56768;
        color: white;
        font-size: 17px;
        font-weight: 600;
        padding: 23px 45px;
        border-radius: 50px;
    }

    .law-button:hover{
        background-color: #e9d758;
    }
</style>