<template>
  <nav id="nav">
    <img src="../assets/logo.png" alt="Logo" />
  </nav>
</template>

<style scoped>
#nav {
  width: 100%;
  background-color: #000;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
#nav > img {
  width: 300px;
}
</style>

<script lang="ts">
import { Vue } from "vue-class-component";
export default class Navigation extends Vue {}
</script>