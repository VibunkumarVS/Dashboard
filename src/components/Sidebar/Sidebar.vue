<template>
    <div class="sidebar_container">
        <h1> Axountee </h1>
        <Account class="accContainer"/>
        <ul>
            <li>Dashboard</li>
            <li>Payments</li>
            <li>Invoices</li>
            <li>Transactions</li>
            <li>Account</li>
        </ul>
    </div>
</template>


<script>

import Account from './Account.vue';

export default {
    name: 'Sidebar' ,
    components : {
        Account
    }
}
</script>

<style scoped>
.sidebar_container{
    width: 15%;
    margin: 0px 0 0 3%;
    padding-top: 50px;
    border-right: 0.3px solid rgb(201, 201, 201);
}

ul{
    list-style: none;
    margin: 0;
    padding: 0;
}

li{
    margin: 30px 0;
}

.accContainer{
    margin: 20px 0;
}

h1{
    color: darkblue;
}

</style>