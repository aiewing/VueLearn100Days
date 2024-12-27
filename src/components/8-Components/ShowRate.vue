<template>
    <h5>你的评分是：{{ score }}</h5>
    <!-- <Rate :value="score" theme="green" @update-rate="update">课程评分</Rate> -->
    <Rate v-model="score">课程评分</Rate>
</template>

<script setup>
import { ref } from 'vue';
import Rate from './Rate.vue';

let score = ref(3.5)
// function update(num) {
//     score.value = num
// }
</script>