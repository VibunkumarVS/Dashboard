<template>
    <div class="container">
        <!-- <BalanceInfo 
            :amount='100'
            :amountLabel = "'TotalBalance'" />
        <BalanceInfo 
            :amount='40'
            :amountLabel = "'Expense'" />
        <BalanceInfo 
            :amount='20'
            :amountLabel = "'Income'" /> -->

    <div class="sort">
        <p> Newest </p>
    </div>
        <Lists />

    </div>
</template>

<script>

import Lists from './Lists.vue';

export default {
    name : 'MainBoard',
    components : {
        Lists
    }
}
</script>

<style scoped>

.sort{
    padding: 0px 20px 0px 0px ;
    width:fit-content;
}   

</style>