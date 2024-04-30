<template>
    <div class="time">
        
    </div>
</template>

<script setup>
import { inject } from 'vue';

const time = inject('time')
console.log(time.value);


</script>

<style scoped>
/* Your component styles here */
</style>