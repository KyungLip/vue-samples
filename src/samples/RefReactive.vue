
<script setup lang="ts">
import { ref } from 'vue';

const msg=ref(0)
msg.value=10
console.log("msg：",msg)
function increment(){
    msg.value++
}
</script>

<template>
    <div class="content">
        <p>Ref：{{ msg }}</p>
        <!-- <button @click="msg++">Add</button> -->
        <button @click="increment">Add</button>

    </div>
</template>
    
<style scoped>

.content{
    height: 100pt;
    background-color: aqua;
    border-radius: 8pt;
    padding-left: 5pt;
    padding-top: 5pt;
}
</style>