<script>
import {defineComponent} from 'vue'
import SideCard from "@/components/SideCard.vue";

export default defineComponent({
  name: "PageSide",
  components: {SideCard}
})
</script>

<template>
  <div>
    side
    <br>
    <side-card></side-card>
    <side-card></side-card>
    <side-card></side-card>
    <side-card></side-card>
    <side-card></side-card>
    <side-card></side-card>
  </div>
</template>

<style scoped>

</style>