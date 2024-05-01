<script setup>// 响应式API

    import { ref ,onMounted} from 'vue'

    const count = ref(0) 

    function increment() {
        count.value++;
    }

    onMounted(()=>{
        console.log("vue 已经挂载完毕了")
    })

</script>

<template>

    <button v-on:click="increment"> count:{{ count }}</button>

</template>


<style></style>