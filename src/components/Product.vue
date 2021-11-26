<template>
  <div class="product">
    <p>Product: {{ name }}</p>
    <img src="../assets/products/1.jpg" :alt="name" />
  </div>
</template>

<style scoped></style>

<script lang="ts">
import { Vue, Options } from "vue-class-component";

@Options({
  props: {
    name: String,
    src: String,
  },
})
export default class Product extends Vue {
  name!: string;
  src!: string;
}
</script>