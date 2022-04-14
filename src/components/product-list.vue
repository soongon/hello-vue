<template>
  <p>
    <button @click="getDataFromServer()">데이터 가져오기</button>
  </p>
  <ul>
      <li v-for="post in products" :key="post.id">
        <p>글번호: {{ post.id }}</p>
        <p>{{ post.title }}</p>
      </li>
    </ul>
</template>

<script>
import axios from 'axios';
export default {
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
      products: [],
    };
  }
}
</script>

<style>

</style>