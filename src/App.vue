<script>
  import Navbar from './components/Navbar.vue'
  import Hero from './components/Hero.vue'
  import Faculty from './components/Faculty.vue';
  import University from './components/University.vue';
  import NewCourses from './components/NewCourses.vue';

  export default {
    components:{
      Navbar,
      Hero,
      Faculty,
      University,
      NewCourses
    }
  }
</script>

<template>
  <Navbar/>
  <Hero/>
  <Faculty/>
  <University/>
  <NewCourses/>
  
</template>

<style>

</style>
