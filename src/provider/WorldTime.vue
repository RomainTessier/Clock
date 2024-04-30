<script setup>
import { provide, inject, watchEffect, ref } from 'vue'


const timeData = ref(null);
provide('time', timeData);

watchEffect(async () => {
    if (inject('ip')) {
        const ip = await inject('ip');
        timeData.value = await getWorldTimeApi(ip);
    }
})

const getWorldTimeApi = async (ip) => {  
    const fetchTime = await fetch(`http://worldtimeapi.org/api/ip/${ip.ip}`);
    const fetchTimeJson = await fetchTime.json();
    return fetchTimeJson;
}
</script>

<template>
    <slot v-if={timeData}>

    </slot>
    <div class="loading" v-else>
      Loading
    </div>
</template>


