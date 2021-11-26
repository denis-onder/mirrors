<template>
  <div>
    <div class="hello">
      <h1>We make IT happen.</h1>
    </div>
    <div class="actions">
      <router-link
        class="button"
        style="margin-right: 12px"
        :to="{ name: 'About' }"
        >About Us
      </router-link>
      <router-link
        class="button"
        style="margin-left: 12px"
        :to="{ name: 'Products' }"
        >Products</router-link
      >
    </div>
  </div>
</template>

<style scoped>
.button {
  background-color: rgb(38, 214, 214);
  color: black;
  padding: 0.75rem 1.25rem;
  border-radius: 4px;
  text-decoration: none;
  font-weight: bold;
}
</style>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({})
export default class HelloWorld extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  text-align: center;
}
.actions {
  width: 100%;
  text-align: center;
}
</style>
