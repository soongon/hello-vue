<template>
  <h3>{{ title }}</h3>
  <p>
    <button @click="buttonClicked()">눌러주세요</button>
  </p>
</template>

<script>
export default {
  methods: {
    buttonClicked() {
      console.log('button clicked...');
      this.title = '버튼이 클릭되어 변수 교체...';
    }
  },
  data() {
    return {
      title: '상품목록이에요..',
    }
  }
}
</script>

<style>

</style>