<script setup>
import WorldTime from './provider/WorldTime.vue';
import Ip from './provider/Ip.vue';
import MainView from './MainView.vue';

</script>

<template>
  <Ip>
    <WorldTime >
     <MainView />
    </WorldTime> 
  </Ip>
</template>

<style scoped>


</style>
