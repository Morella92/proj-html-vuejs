<script>
    export default {

    }
</script>

<template>
    <section class="university-section">
        <div class="container-small">
            
            <div class="row-column">
                <img class="clock-img" src="../../public/img/Clock-and-Bell.png" alt="">
                <h2 class="section-title">University Year</h2>
            </div>
            
            <div class="row">
                <div class="col">
                    <h4 class="info-title">Demo Classes</h4>
                    <p class="info-p">
                        In the first week, students try to accomodate with the teaching style and choose their optional courses.
                    </p>
                </div>
                <div class="col">
                    <h4 class="info-title">Graduation Day</h4>
                    <p class="info-p">
                        On the day of graduation, all students gather for the ceremony and then network and party among others.
                    </p>
                </div> 
            </div>

            <img class="timeline-img" src="../../public/img/Timeline-Item.png" alt="">

            <div class="row">
                <div class="col">
                    <h4 class="info-title">Orientation</h4>
                    <p class="info-p">
                        First day of university year, all students gather for the opening ceremony and then networks with others.
                    </p>
                </div>
                <div class="col">
                    <h4 class="info-title">Evaluation</h4>
                    <p class="info-p">
                        At the end of the semester, students take a general evaluation test for every subject they're learning.
                    </p>
                </div> 
            </div>

            <div class="row-column">
                <img class="calendar-img" src="../../public/img/upcoming-events-calendar-icon.png" alt="">
                <h2 class="section-title">Upcoming Events</h2>
            </div>

            <div class="row">
                <div class="col-event">
                    <h3 class="event-title">Coaching Sessions</h3>
                    <p class="event-date">
                        <i class="fa-sharp fa-regular fa-calendar-days"></i>
                        <span class="date">20 May 21:30 PM</span>
                    </p>
                    <p class="event-p">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor[...]
                    </p>
                    <button class="event-button">
                        <i class="fa-solid fa-plus"></i>
                        <span>Find more </span>
                    </button>
                </div>
                <div class="col-event">
                    <h3 class="event-title">Coaching Sessions</h3>
                    <p class="event-date">
                        <i class="fa-sharp fa-regular fa-calendar-days"></i>
                        <span class="date">24 Mar 18:00 PM</span>
                    </p>
                    <p class="event-p">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor[...]
                    </p>
                    <button class="event-button">
                        <i class="fa-solid fa-plus"></i>
                        <span>Find more </span>
                    </button>
                </div>
                <div class="col-event">
                    <h3 class="event-title">Coaching Sessions</h3>
                    <p class="event-date">
                        <i class="fa-sharp fa-regular fa-calendar-days"></i>
                        <span class="date">12 Feb 13:30 PM</span>
                    </p>
                    <p class="event-p">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor[...]
                    </p>
                    <button class="event-button">
                        <i class="fa-solid fa-plus"></i>
                        <span>Find more </span>
                    </button>
                </div>
            </div>

            <div class="row-column">
                <button class="all-events">View All Events</button>
            </div>
        </div>
        
        <img class="university-wave" src="../../public/svg/svg-1.svg" alt="">
    </section>

</template>

<style scoped>
    .university-section{
        background-color: #E56768;
        margin-top: -5px;
    }

    .row-column{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .clock-img, .calendar-img{
        width: 70px;
        margin-top: 100px;
    }

    .section-title{
        font-size: 48px;
        font-weight: 600;
        color: white;
        margin: 20px 0 10px;
    }

    .row{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 90px;
    }

    .info-title{
        color: white;
        font-size: 18px;
        font-weight: 600;
        margin-top: 50px;
        text-align: center;
        padding: 20px 0 10px;
    }

    .info-p{
        font-size: 16px;
        color: white;
        text-align: center;
    }

    .timeline-img{
        margin: 20px 0; 
    }

    .col-event{
        margin-top: 55px;
        background-color: white;
        color: #3D404F;
        border-radius: 14px;
        padding: 15px 30px;
        text-align: center;
        position: relative;
    }

    .event-title{
        font-size: 28px;
        font-weight: 600;
        margin-top: 25px;
    }

    .event-date{
        font-size: 14px;
        margin: 10px;
    }

    .date{
        margin-left: 5px;
    }
    .event-p{
        font-size: 16px;
        margin-bottom: 40px;
    }

    .event-button{
        background-color: #E56768;
        color: white;
        padding: 8px 16px;
        border-radius: 20px;
        font-size: 14px;
        font-weight: 600;
        position: absolute;
        left: 110px;
        box-shadow: 1px 1px 1px #dedede;
    }

    .event-button:hover{
        background-color: #e9d758;
    }

    .all-events{
        background-color: #e9d758;
        color: white;
        font-weight: 600;
        font-size: 14px;
        padding: 23px 45px;
        border-radius: 35px;
        margin: 55px 0;
    }

    .all-events:hover{
        background-color: #E56768;
    }

    .university-wave{
        margin: -88px;
        width: 1600px;
    }
</style>