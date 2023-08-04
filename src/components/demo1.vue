<template>
    <div class="btn">
        button
    </div>
</template>

<script>
export default {
    name: "demo1"
}
</script>

<style>
.btn {
    width: 200px;
    height: 50px;
    background: red;
    border-radius: 10px;
    text-align: center;
    cursor: pointer;
    box-shadow: 0, 3px 5px #aaa;
}

.btn :hover {
    background: blue;
}
</style>