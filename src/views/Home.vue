<template>
  <div class="home">
    <h1>ようこそ!!<br>Kosuke Itamotoのポートフォリオサイトへ</h1>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '../components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
  }
}
</script>

<style scoped>
.home{
  height: 1000px;
}
h1{
  margin: 200px auto;
}
</style>