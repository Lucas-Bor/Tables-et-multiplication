<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" width="100" height="100">
    <nav>
      <router-link to="/">&nbsp;Home |</router-link>
      <router-link to="/tables">&nbsp;Les tables |</router-link>
      <router-link to="/TaMultiplication">&nbsp;Ta propre multiplication</router-link>
    </nav>
    <router-view />
  </div>
</template>

<script>
  export default {
    name: "app"
  };
</script>

<style>
  #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

</style>
