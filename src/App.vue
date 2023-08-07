<template>
  <div class="home">
    <h1 style="text-align: center">This is templete</h1>
    <br>
    <button @click="one()"> 打印1</button>
    <button @click="two()"> 打印2</button>
    <br>
    {{ message }} <!--变量-->
    <br>
    {{ arr[1] }}
    <br>
    {{ arr[2] }}
    <br>
    {{ arr[0] }}
    <br>
    {{ obj.author }}
    <br>
    <div v-once>{{ num }}</div>
    <button @click="num++">+</button>
    <hr>

    <div v-pre>
      {{num}}
    </div>

    <div v-html="link"></div>

    <a :href="url">vuejs</a>

    <demo1></demo1>
  </div>
</template>

<script>
import demo1 from './components/demo1.vue'

export default {
  name: "App",
  data() {
    return {
      link: "<a href='https://www.bilibili.com'>bilibili</a>",
      num: 0,
      message: "Hahhahahha",
      arr: ['python', 'ruby', 'php'],
      obj: {
        name: 'vscode',
        author: 'Microsoft',
      },
      url: 'https://www.vuejs.org',
    }
  },
  methods: {
    one() {
      console.log('1111')
    },
    two() {
      console.log('222')
      console.log(this.message)
    }
  },
  components: {
    demo1
  }
}
</script>

<style>
.home {
  width: 300px;
  height: 300px;
  background: yellow;
}
</style>
