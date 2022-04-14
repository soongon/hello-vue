<template>
  <main>
    <product-title></product-title>
    <product-list></product-list>
  </main>
</template>

<script>
import ProductList from './product-list.vue'
import productTitle from './product-title.vue'
export default {
  components: { 
    productTitle,
    ProductList 
  },

}
</script>

<style>

</style>