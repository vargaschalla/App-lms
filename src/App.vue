<template>
  <div class="appx">
    <p>WELCOME</p>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome" msg2="Hola "/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
.appx {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.appx p{
  color: #006356;
  font-family: times new roman, Helvetica, Arial, sans-serif;
}
</style>
