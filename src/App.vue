<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About me</router-link>
      <router-link to="/works">Works</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
    <transition name="aaa" mode="out-in">
      <router-view/>
    </transition>
  </div>
</template>

<style>
body{
  margin: 0px;
}

#app {
  font-family: sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #000044;
  text-align: center;
  margin-top: 60px;
}

h1{
  font-family: sans-serif;
  font-size: 50px;
  color: #000044;
  text-shadow: 2px 2px 2px #bbb;
}

#nav {
  padding: 10px;
  border-bottom: 1px solid #ccc;
  background-color: #fff;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
}

#nav a {
  font-weight: bold;
  color: #000044;
  padding: 0 50px;
  text-decoration: none;
  font-size: 25px;
  text-shadow: 2px 2px 2px #aaa;
  user-select: none;
}

#nav a:hover{
  color: #3399FF;
  border-bottom: 1px solid #3399FF;
  padding-bottom: 17px;
}

#nav a.router-link-exact-active {
  color: #3399FF;
  border-bottom: 1px solid #3399FF;
  padding-bottom: 17px;
}

.aaa-enter-active, .aaa-leave-active {
  transition: 0.5s;
}

.aaa-enter, .aaa-leave-to {
  opacity: 0;
}
</style>
