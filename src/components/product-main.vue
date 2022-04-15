<template>
  <main>
    <product-title 
      :isShow="isShow" 
      :title="title"></product-title>
    <product-list :products="products"></product-list>
  </main>
</template>

<script>
import ProductList from './product-list.vue';
import productTitle from './product-title.vue';
import axios from 'axios';

export default {
  components: { 
    productTitle,
    ProductList 
  },
  created() {
    this.getDataFromServer();
  },
  methods: {
    async getDataFromServer() {
      axios.get('https://jsonplaceholder.typicode.com/posts')
        .then(res => {
          console.log(res.data);
          this.products = res.data;
        });
    }
  },
  data() {
    return {
      isShow: true,
      title: '상품목록이에요..',
      products: [],
    }
  }

}
</script>

<style>

</style>