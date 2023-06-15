<template>
  <div id="page-wrap">
    <ProductsGrid :products="products" />
  </div>
</template>
<script>
import ProductsGrid from "@/components/ProductsGrid.vue";
import { products } from "../fake-data.js";
export default {
  components: { ProductsGrid },
  name: "ProductsPage",
  data() {
    return {
      products,
    };
  },
};
</script>
