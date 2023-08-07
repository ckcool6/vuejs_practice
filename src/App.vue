<template>
  <div class="page">
    <!--
        <h1 style="text-align: center">This is templete</h1>
        <br>
        <button @click="one()"> 打印1</button>
        <button @click="two()"> 打印2</button>
        <br>
        {{ message }} &lt;!&ndash;变量&ndash;&gt;
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
    -->

    <!--    <demo1></demo1>-->
    <!--    <demo2></demo2>-->

    <div class="header">
      <page-header></page-header>
    </div>

    <div class="main">
      <page-main></page-main>
    </div>

    <div class="side">
      <page-side></page-side>
    </div>
  </div>
</template>

<script>
import demo1 from './components/demo1.vue'
import Demo2 from "@/components/demo2.vue";
import PageHeader from "@/components/PageHeader.vue";
import PageMain from "@/components/PageMain.vue";
import PageSide from "@/components/PageSide.vue";

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
    PageSide,
    PageMain,
    PageHeader,
    Demo2,
    demo1
  }
}
</script>

<style lang="scss">
.page {

  .header {
    width: 100%;
    height: 100px;
    background-color: #EFEFEF;
    float: left;
    margin-bottom: 20px;
  }

  .main {
    width: 75%;
    height: 800px;
    background-color: #EFEFEF;
    float: left;
    margin-top: 30px;
  }

  .side {
    width: 20%;
    height: 800px;
    background-color: #EFEFEF;
    float: right;
    margin-top: 30px;
  }

}
</style>
