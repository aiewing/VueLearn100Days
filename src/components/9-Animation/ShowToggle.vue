<template>

    <button @click="toggle">Click</button>
    <transition name="fade">
        <h1 v-if="showToggle">Hello Vue 3</h1>
    </transition>
</template>

<script setup>
import { ref } from 'vue';
let showToggle = ref(true)
function toggle() {
    showToggle.value = !showToggle.value
}
</script>

<style>
.fade-enter-active,
.fade-leave-active {
    transition: opacity 0.5s linear;
}

.fade-enter-from,
.fade-leave-to {
    opacity: 0;
}
</style>