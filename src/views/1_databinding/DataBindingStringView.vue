<template>
  <div><!--최상위 루트태그를 사용하는것이 좋다. vue2버전에서는 오류임-->
    <h1>Hello {{ userName }}</h1>
    <p> {{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'JunYoung',
      message: 'Weblcome JHSE Blog'
    }
  },
  name: 'DataBindingStringView'
}
</script>

<style scoped>

</style>
