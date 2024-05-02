<script setup>
import Time from './components/Time.vue';
</script>

<template>
    <div class="quoteContainer">Quote</div>
    <div class="hourContainer">
        <Time />
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;900&display=swap');


#app{
    height: 100dvh;
    background-image: linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url('./assets/desktop/bg-image-daytime.jpg');
    background-position: center;
    backdrop-filter: brightness(0.5);
    font-family: 'Inter', sans-serif;
}

body, html{
    padding: 0;
    margin: 0;
}

body{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    
}

#app {
    padding: 25px;
}

#app > div{
    height: 50%;
}
</style>