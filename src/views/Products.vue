<template>
  <div class="container">
    <div class="products">
      <div class="product">
        <p>Product: 1</p>
        <img src="../assets/products/1.jpg" :alt="name" />
      </div>

      <div class="product">
        <p>Product: 2</p>
        <img src="../assets/products/2.jpg" :alt="name" />
      </div>

      <div class="product">
        <p>Product: 3</p>
        <img src="../assets/products/3.jpg" :alt="name" />
      </div>

      <div class="product">
        <p>Product: 4</p>
        <img src="../assets/products/4.jpg" :alt="name" />
      </div>

      <div class="product">
        <p>Product: 5</p>
        <img src="../assets/products/5.jpg" :alt="name" />
      </div>

      <div class="product">
        <p>Product: 6</p>
        <img src="../assets/products/7.jpg" :alt="name" />
      </div>

      <div class="product">
        <p>Product: 7</p>
        <img src="../assets/products/7.jpg" :alt="name" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  height: 100%;
}
.products {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 24px;
}
.product {
  border: 1px solid black;
  text-align: center;
}
.product p {
  margin-left: 8px;
  text-align: left;
  font-weight: bold;
}
.product img {
  max-width: 300px;
  max-height: 175px;
}
</style>

<script lang="ts">
import { Vue, Options } from "vue-class-component";

@Options({})
export default class Products extends Vue {
  get products(): any[] {
    const payload = [];

    for (let i = 1; i <= 7; i++) {
      payload.push({
        name: `${i}`,
      });
    }

    return payload;
  }
}
</script>