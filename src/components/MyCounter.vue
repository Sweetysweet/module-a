<script setup>
import { ref } from 'vue'
const counter = ref(0)

const countHandler = () => {
    counter.value++
}
const userName = ref('')
</script>
<template>
<div>
    <span>Счетчик: {{counter}}</span>
    <span>Андрей</span>
    <button @click="countHandler">+1</button>
    <div style="margin-top: 10px;">
        <input type="text" v-model="userName">
    </div>
</div>
</template>