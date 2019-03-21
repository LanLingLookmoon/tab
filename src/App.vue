<template>
  <div id="app">
    <tab></tab>
  </div>
</template>

<script>
// 引入地址
import HelloWorld from "./components/HelloWorld";
import tab from "./components/pages/tab";
export default {
  name: "App",
  components: {
    tab
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
* {
  margin: 0;
  padding: 0;
}
</style>
