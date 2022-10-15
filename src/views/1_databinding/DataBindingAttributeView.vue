<template>
  <div>
    <input type="text" name="" id="" v-bind:value="userId" readonly> <!--attribute 에 바인딩-->
    <input type="text" name="" id="" :value="userId" readonly> <!--v-bind 생략가능-->
    <br>
    <img :src="imgSrc" alt="" style="width: 100px; height:auto;">
    <br>
    <input type="search" name="" id="" v-model="txt1">
    <button :disabled="txt1 === ''">조회</button>
  </div>
</template>

<script>
export default {
  name: 'DataBindingAttributeView',
  data() {
    return {
      userId: 'JunYoung',
      imgSrc: 'https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png',
      txt1: ''
    }
  }
}
</script>

<style scoped>

</style>
