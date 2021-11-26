<template>
  <div class="app-container">
    <Navigation />
    <router-view />
  </div>
</template>

<style>
html {
  min-height: 100vh;
}
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}
.app-container {
  height: 100vh;
}
</style>

<script lang="ts">
import { Vue, Options } from "vue-class-component";
import Navigation from "./components/Navigation.vue";

@Options({
  components: {
    Navigation,
  },
})
export default class App extends Vue {}
</script>