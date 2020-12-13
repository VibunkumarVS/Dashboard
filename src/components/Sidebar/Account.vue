<template>
<div class="root_container">

    <div class="account_header"> 
        <img class="accName" src="../../assets/logo.png"/>
        <div class="dropdown"> Vibunkumar </div>
    </div>
    <h2> $ 1000 </h2>
</div>

</template>


<script>
export default {
    name: "Account"
}
</script>

<style scoped>

.root_container{
    padding: 30px 0;
}

.account_header, .dropdown {
    display: inline-block;
}

.dropdown{
    margin-left: 5px;
}

.accName{
    height: 15px;
    width: 15px;
}

h2{
    margin: 0;
}

</style>