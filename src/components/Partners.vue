<script>
    export default {
        data(){
            return{
                partners:[
                    '../../public/img/partner-2.png',
                    '../../public/img/partner-3.png',
                    '../../public/img/partner-4.png',
                    '../../public/img/partner-5.png',
                    '../../public/img/partner-6.png',
                    '../../public/img/partner-8.png',
                    '../../public/img/partner-1.png',
                    '../../public/img/partner-7.png'
                ],
                scaledPartners: [
                    '../../public/img/partner-3.png',
                    '../../public/img/partner-4.png',
                    '../../public/img/partner-6.png',
                    '../../public/img/partner-8.png',
                    '../../public/img/partner-1.png'
                ]
            }
        }
    }
</script>

<template>
    <section class="partners-section">
        <h2 class="partners-title">Partners</h2>
        <p class="partners-p">
            Leverage agile frameworks to provide a robust synopsis for high level overviews. <br> Iterative approaches to corporate strategy.
        </p>
        <ul class="partners-icon">
            <li v-for="partner in partners">
                <img :src="partner" v-if="scaledPartners.includes(partner)"
                :class="{'partners-img': true, 'small-img': scaledPartners.includes(partner)}">
                <img :src="partner" v-else
                :class="{'partners-img': true, 'large-img': !scaledPartners.includes(partner)}">
            </li>
        </ul>

        <img class="wave-partners" src="../../public/img/background-wave3.png" alt="">
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .partners-section{
        margin-top: 33px;
    }

    .partners-title{
        font-size: 48px;
        font-weight: 600;
        color: $text-color;
        text-align: center;
    }

    .partners-p{
        font-size: 16px;
        color: $text-color;
        text-align: center;
        margin: 28px 0;
    }

    .partners-icon{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 25px;
        filter: invert(80%);
    }

    .small-img {
        width: 70px;
    }

    .large-img {
        width: 120px;
    }

    .small-img:hover, .large-img:hover{
        filter: invert(1);
    }
    .wave-partners{
        background-color: #e4e5e7;
        height: 150px;
    }
</style>