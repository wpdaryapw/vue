<script>
  import Header from './components/Header.vue'
  import Main from './components/Main.vue'
  import Skills from './components/Skills.vue'
  import Contacts from './components/Contacts.vue'
  export default {
    components: {Header, Main, Skills, Contacts}
  }
</script>

<template>
  <Header></Header>
  <Main></Main>
  <Skills></Skills>
  <Contacts></Contacts>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Abel&display=swap');

  *{
    margin: 0;
    padding: 0;

  }
</style>
