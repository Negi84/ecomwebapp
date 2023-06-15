<template>
  <div class="grid-wrap">
    <ProductsGridItems v-for="product in products" :key="product.id" :product="product" />
  </div>
</template>

<script>
import ProductsGridItems from "./ProductsGridItems.vue";
export default {
  name: "ProductsGrid",
  components: {
    ProductsGridItems,
  },
  props: ["products"],
};
</script>
<style scoped>
.grid-wrap {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-top: 16px;
}
</style>
