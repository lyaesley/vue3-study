<template>
  <div>
    <!--2가지 방식 가능-->
    <input type="search" name="" id="" @keyup="checkEnter($event)" v-model="searchText">

    <input type="search" name="" id="" @keyup.enter="doSearch()" v-model="searchText">
    <button @click="doSearch">조회</button>
    <button type="submit" @click.prevent="doSearch()">조회</button>
  </div>
</template>

<script>
// .stop - event.stopPropagation() 과 동일 기능
// .prevent - event.preventDefault() 과 동일기능
export default {
  name: 'EventKeyView',
  data() {
    return {
      searchText: ''
    }
  },
  methods: {
    doSearch() {
      console.log(this.searchText)
    },
    checkEnter(event) {
      if (event.keyCode === 13) {
        this.doSearch()
      }
    }
  }
}
</script>

<style scoped>

</style>
