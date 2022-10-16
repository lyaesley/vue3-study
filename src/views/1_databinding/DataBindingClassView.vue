<template>
  <div>
    <div>
      <div :class="{'text-red':hasError, active:isActive}">클래스 바인딩</div>
      <div :class="class2">클래스 바인딩2</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DataBindingClassView',
  data() {
    return {
      isActive: true,
      hasError: false,
      class2: ['active', 'text-red']
    }
  }
}
</script>

<style scoped>
.active {
  background-color: greenyellow;
  font-weight: bold;
}

.text-red {
  color: red;
}
</style>
