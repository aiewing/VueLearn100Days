<template>
    <h1 @click="toggle">click</h1>
</template>

<script setup>
import { useFullscreen } from '@vueuse/core';

const { toggle } = useFullscreen()
</script>