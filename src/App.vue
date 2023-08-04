<template>
    <div class="home">
        this is app templete
        <br>
        <button @click="one()"> 打印1</button>
        <button @click="two()"> 打印2</button>
        <br>
        {{ message }}
        <br>
        <demo1></demo1>
    </div>
</template>

<script>
import demo1 from './components/demo1.vue'

export default {
    name: "App",
    data() {
        return {
            message: "hahhahahha"
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
