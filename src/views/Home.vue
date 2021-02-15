<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Codey Du's 2020FEB12 Vue.js App"/>
    <h1>Current Environment: {{ checkEnv }}</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  computed: {
    checkEnv() {
      return process.env.NODE_ENV
    }
  }
}
</script>
