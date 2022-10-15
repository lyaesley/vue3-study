<template>
  <div>
    <input type="text" v-model="userId">
    <button @click="myFun">클릭</button>
    <button @click="changeData">변경</button>
    <br>
    <input type="text" v-model="num1"/> +
    <input type="text" v-model="num2"/> =
    <span>{{num1 + num2}}</span>
    <br>
    <input type="text" v-model.number="num3"/> +
    <input type="text" v-model.number="num4"/> =
    <span>{{num3 + num4}}</span>
  </div>
</template>

<script>
export default {
  name: 'DataBindingInputView',
  data() {
    return {
      userId: 'JunYoung',
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0

    }
  },
  methods: {
    myFun() {
      console.log(this.userId)
    },
    changeData() {
      this.userId = 'JunYoung'
    }
  }
}
</script>

<style scoped>

</style>
