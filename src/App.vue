<script>
  import Navbar from './components/Navbar.vue';
  import Hero from './components/Hero.vue';
  import Faculty from './components/Faculty.vue';
  import University from './components/University.vue';
  import NewCourses from './components/NewCourses.vue';
  import Subscribe from './components/Subscribe.vue';
  import Partners from './components/Partners.vue';
  import Footer from './components/Footer.vue';

  export default {
    components:{
      Navbar,
      Hero,
      Faculty,
      University,
      NewCourses,
      Subscribe,
      Partners,
      Footer
    }
  }
</script>

<template>
  <Navbar/>
  <Hero/>
  <Faculty/>
  <University/>
  <NewCourses/>
  <Subscribe/>
  <Partners/>
  <Footer/>
  
</template>

<style>

</style>
