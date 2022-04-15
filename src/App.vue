<template>
  <product-header>SNS</product-header>
  <product-main></product-main>
  <product-footer></product-footer>
  <kitri-button>click me</kitri-button>
</template>

<script>
import ProductFooter from './components/product-footer.vue'
import ProductHeader from './components/product-header.vue'
import ProductMain from './components/product-main.vue'
import KitriButton from './global-components/kitri-button.vue'

export default {
  name: 'App',
  components: {
    ProductHeader,
    ProductMain,
    ProductFooter,
    KitriButton
  }
}
</script>

<style>

</style>
