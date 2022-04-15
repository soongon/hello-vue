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
export default {
  props: [
    'products',
  ],
}
</script>

<style>

</style>