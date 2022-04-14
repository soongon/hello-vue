<template>
  <product-header></product-header>
  <product-main></product-main>
  <product-footer></product-footer>
</template>

<script>
import ProductFooter from './components/product-footer.vue'
import ProductHeader from './components/product-header.vue'
import ProductMain from './components/product-main.vue'

export default {
  name: 'App',
  components: {
    ProductHeader,
    ProductMain,
    ProductFooter
  }
}
</script>

<style>

</style>
