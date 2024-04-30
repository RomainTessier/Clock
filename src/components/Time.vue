<script setup>
import { inject } from 'vue';

const time = inject('time')
console.log(time.value.datetime.slice(11, 16));

const hour = time.value.datetime.slice(11, 16);
</script>


<template>
    <div class="time">
        <div class="hour">{{hour}}</div>
    </div>
</template>



<style scoped>
/* Your component styles here */
</style>