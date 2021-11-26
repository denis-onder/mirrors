<template>
  <div>
    <div class="hello">
      <h1>We make IT happen.</h1>
    </div>
    <div class="actions">
      <router-link style="margin-right: 12px" :to="{ name: 'About' }"
        >About Us
      </router-link>
      <router-link style="margin-left: 12px" :to="{ name: 'Products' }"
        >Products</router-link
      >
    </div>
  </div>
</template>

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
