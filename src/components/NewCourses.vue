<script>
    export default {
        data(){
            return{

                NewCourseName:[
                    'Make Better Decisions',
                    'How to be a speaker',
                    'Network Introductions',
                    'Brand Management'
                ],

                NewCourseImage: [
                    '../../public/img/Decisions-icon.png',
                    '../../public/img/Speaker-icon.png',
                    '../../public/img/Network-icon.png',
                    '../../public/img/Brand-icon.png'
                ]
            }
        }
    }
</script>

<template>
    <section class="new-courses-section">
        <div class="container-small">
            <h2 class="new-courses-title">Latest Courses</h2>

            <ul class="row">
                <li v-for="(name, index) in NewCourseName" :key="index" class="new-course-list">
                    <a href="#">
                        <img :src="NewCourseImage[index]" class="new-course-images">
                        <h4 class="new-course-name">{{ name }}</h4>
                        <p class="new-courses-p">
                            <i class="fa-regular fa-user"></i>
                            <span class="new-courses-span">Teacher: <strong>James Colins</strong></span>
                        </p>
                        <p class="new-courses-p">
                            <i class="fa-regular fa-money-bill-1"></i>
                            <span class="new-courses-span">Price: <strong>Free</strong></span>
                        </p>
                        <button class="new-courses-button">
                            <i class="fa-solid fa-eye"></i>
                            View Course
                        </button>
                    </a>
                </li>
            </ul>

            <div class="row-exam">
                <div class="col-exam">
                    <img class="exam-img" src="../../public/img/Exam-icon.png" alt="">
                    <h2 class="exam-title">
                        The most efficient <br>examination method
                    </h2>
                    <p class="exam-p">
                        EduPrime has gathered teachers from around the globe to <br> brainstorm in order to facilitate the evaluation of our students. 
                        <br> Every teacher from our university has an influence on how <br> students are evaluated at his/her subject.
                    </p>
                    <button class="exam-button">Discover the Method</button>
                </div>
                <div class="col">
                    <img class="exam-illustration" src="../../public/img/Exam-Illustration.png" alt="">
                </div>
            </div>

            <div class="row-exam">
                <div class="col">
                    <img class="exam-illustration" src="../../public/img/Girl-Illustration.png" alt="">
                </div>
                <div class="col-exam">
                    <img class="exam-img" src="../../public/img/Exam-icon-1.png" alt="">
                    <h2 class="exam-title">
                        Variable fees <br>for international students.
                    </h2>
                    <p class="exam-p">
                        EduPrime has gathered teachers from around the globe to <br> brainstorm in order to facilitate the evaluation of our students. 
                        <br> Every teacher from our university has an influence on how <br> students are evaluated at his/her subject.
                    </p>
                    <button class="exam-button">List of Fees</button>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .new-courses-section{
        margin-top: 78px;
    }

    .new-courses-title{
        font-size: 48px;
        color: $text-color;
        margin-bottom: 62px;
    }

    .row{
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    .new-course-list{
        padding: 25px 30px 45px;
        text-align: center;
        font-size: 14px;
        line-height: 1.5;
        color: $text-color;
        border: 0.5px solid #EAEAEA;
        box-shadow: 10px 10px 5px #dedede;
        position: relative;
    }

    .new-course-name{
        font-size: 18px;
        margin: 12px 0;
    }
    .new-course-images{
        width: 62px;  
    }

    .new-courses-p{
        margin: 12px 0;
    }

    .new-courses-span{
        margin-left: 5px;
    }

    .new-courses-button{
        font-size: 14px;
        font-weight: 600;
        color: $tertiary;
        background-color: $bg-primary;
        padding: 13px 20px;
        border-radius: 20px;
        position: absolute;
        left: 50px;
        bottom: -15px;
    }

    .new-courses-button:hover, .exam-button:hover{
        background-color: $secondary;
    }

    .row-exam{
        display: flex;
        align-items: center;
        justify-content: space-between;
        
    }

    .col-exam{
        margin-top: 55px;
    }

    .exam-title{
        font-size: 48px;
        color: $text-color;
    }

    .exam-p{
        font-size: 16px;
        color: #8b8b8a;
        line-height: 28px;
        margin-top: 22px;
        margin-bottom: 22px;
    }
    .exam-img{
        width: 39px;
    }

    .exam-button{
        background-color: $bg-primary;
        color: $tertiary;
        padding: 23px 45px;
        border-radius: 35px;
        font-size: 14px;
        font-weight: 600;
    }
    .exam-illustration{
        width: 450px;
        margin-top: 55px;
    }
</style>