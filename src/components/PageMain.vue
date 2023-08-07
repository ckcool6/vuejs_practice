<script>
import {defineComponent} from 'vue'
import MainCard from "@/components/MainCard.vue";

export default defineComponent({
  name: "PageMain",
  date() {
    return {
      ImageDemo1:
    }
  },
  components: {MainCard}
})
</script>

<template>
  <div>
    <main-card></main-card>
    <main-card></main-card>
    <div style="clear:both"></div>
    <br>
    <hr>
    <img :src="ImageDemo1" style="width: 300px; height:400px; float: left">
  </div>
</template>

<style scoped>

</style>