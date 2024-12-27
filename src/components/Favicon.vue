<script setup>
import useFaviocn from '../utils/favicon';
    let {favicon} = useFaviocn()
    
    function loading() {
        favicon.value = '/icon.jpg'
    }
</script>

<template>
    <button @click="loading">123</button>
</template>