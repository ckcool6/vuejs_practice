<script>
export default {
  name: 'demo2',
  data() {
    return {
      myArr: ['1111', '2222', '3333', '4444', '55555'],
      user: {
        name: 'lucy',
        age: 50,
        sex: 'woman',
        birthday: '1999-7-1',
      },

    }
  }
}
</script>

<template>
  <div class="container">

    <div v-for="i in myArr">
      <h2>{{ i }}</h2>
    </div>

    <div v-for="(item,index) in user">
      <h2>{{ item }}---{{ index }}</h2>
    </div>

  </div>
</template>

<style>

</style>