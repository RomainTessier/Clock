<script setup>
import { provide, } from 'vue'

const getIp = async () => {
    const fetchIp = await fetch('https://api.ipify.org?format=json');
    const ip = await fetchIp.json();
    console.log(ip);
    return ip;
    
}

provide('ip', getIp());
</script>

<template>
    <slot>

    </slot>
</template>
