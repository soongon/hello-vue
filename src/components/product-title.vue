<template>
  <h3 v-show="isShow">{{ title }}</h3>
  <p>
    <button @click="buttonClicked()">눌러주세요</button>
  </p>
  <p>
    <input type="text" v-model="textData">
  </p>
  <p>{{ textData }}</p>
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
      textData: 'kim soongon....',
      isShow: true,
      title: '상품목록이에요..',
    }
  }
}
</script>

<style>

</style>