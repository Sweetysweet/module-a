<script setup>
import { ref } from 'vue'
const counter = ref(0)

const countHandler = () => {
    counter.value++
}
</script>
<template>
<div>
    <span>Счетчик: {{counter}}</span>
    <button @click="countHandler">+1</button>
</div>
</template>