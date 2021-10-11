<template>
  <div id="app">
    <MyButton />
    <img alt="Vue logo" src="./assets/logo.png" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import MyButton from "@/components/MyButton.vue";

export default Vue.extend({
  name: "App",
  components: { MyButton },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
