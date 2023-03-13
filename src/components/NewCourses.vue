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
                        <button>View Course</button>
                    </a>
                </li>
            </ul>
        </div>
    </section>

</template>

<style scoped>
    .new-courses-section{
        margin-top: 78px;
    }

    .new-courses-title{
        font-size: 48px;
        color: #3d404f;
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
        color: #434959;
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
</style>