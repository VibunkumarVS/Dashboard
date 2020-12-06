<template>
    <div class='mainContent_Container'>
        <h3>My Dashboard 🐳</h3>
        <MainBoard />
        <Lists />
    </div>
</template>

<script>

import MainBoard from './MainBoard.vue';
import Lists from './Lists.vue';

export default {
    name: 'MainContent',
    components : {
        MainBoard,
        Lists
    }
}
</script>

<style scoped>

.mainContent_Container{
    background-color: crimson;
    height: 100%;
    box-sizing: border-box;
    width: 60%;
    padding: 5px 10px;
}
</style>