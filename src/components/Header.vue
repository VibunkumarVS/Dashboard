<template>
    <div class="container">
        <h1> Your Transaction's </h1>
        <img class="addimg"  src="../assets/logo.png" />
    </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>



.container{
    height: 50px;
    width: 100%;
    padding: 40px 50px;
    display: flex;
}

.addimg{
    width: 40px;
    height: 40px;
    margin: 10px 0px 10px 200px;
}
</style>