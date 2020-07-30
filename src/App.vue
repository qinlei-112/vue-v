<template>
  <div id="app">
    <router-view />
    <!-- <myFooter></myFooter> -->
  </div>
</template>

<script>
import login from "./components/login";

import myFooter from "./components/myFooter";

export default {
  name: "App",
  components: {
    login,
    myFooter
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
