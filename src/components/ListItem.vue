<template>
    <div class="lineItem">
        {{ defaultValue }}
    </div>    
</template>

<script>
export default {
    name: '',
    props: ['defaultValue']
}
</script>

<style scoped>
.lineItem{
    height: 10px;
    margin: 5px 0;
    padding: 3px;
}
</style>

