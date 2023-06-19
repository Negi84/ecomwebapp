<template>
  <div v-if="products.length > 0">
    <ProductsItemsList
      v-for="product in products"
      :key="product.id"
      :product="product"
    />
  </div>
  <p v-else>You haven't added anything to your cart</p>
</template>

<script>
import ProductsItemsList from "./ProductsItemsList.vue";
export default {
  name: "ProductsList",
  components: {
    ProductsItemsList,
  },
  props: ["products"],
};
</script>
