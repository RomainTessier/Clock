<script setup>
import WorldTime from './provider/WorldTime.vue';
import Ip from './provider/Ip.vue';
import Time from './components/Time.vue';
import { inject } from 'vue';


</script>

<template>
  <Ip>
    <WorldTime >
     <Time />
    </WorldTime> 
  </Ip>
</template>
