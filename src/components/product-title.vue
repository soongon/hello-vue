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
  props: {
    isShow: {
      type: Boolean,
      required: true,
    },
    title: {
      type: String,
      default() {
        return 'no title';
      }
    }
  },
  data() {
    return {
      textData: '',
    }
  },
  methods: {
    buttonClicked() {
      console.log('button clicked...');
      this.title = '버튼이 클릭되어 변수 교체...';
    }
  },
}
</script>

<style>

</style>