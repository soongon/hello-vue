<template>
  <ul>
      <li>{{ products[0] }}</li>
      <li>{{ products[1] }}</li>
      <li>{{ products[2] }}</li>
    </ul>
</template>

<script>
export default {
  data() {
    return {
      products: ['아이폰13', '갤럭시22', '모니터27'],
    };
  }
}
</script>

<style>

</style>