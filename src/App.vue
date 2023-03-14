<script>
  import NavbarApp from './components/NavbarApp.vue';
  import Hero from './components/Hero.vue';
  import Faculty from './components/Faculty.vue';
  import University from './components/University.vue';
  import NewCourses from './components/NewCourses.vue';
  import Subscribe from './components/Subscribe.vue';
  import Partners from './components/Partners.vue';
  import FooterApp from './components/FooterApp.vue';

  export default {
    components:{
      NavbarApp,
      Hero,
      Faculty,
      University,
      NewCourses,
      Subscribe,
      Partners,
      FooterApp
    }
  }
</script>

<template>

  <section>
    <NavbarApp/>
    <Hero/>
    <Faculty/>
    <University/>
    <NewCourses/>
    <Subscribe/>
    <Partners/>
    <FooterApp/>
  </section>
  
</template>

<style>

  section{
    overflow-x: hidden;
  }
</style>
