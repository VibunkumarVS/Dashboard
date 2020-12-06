<template>
    <div class="container">
        <BalanceInfo 
            :amount='100'
            :amountLabel = "'TotalBalance'" />
        <BalanceInfo 
            :amount='40'
            :amountLabel = "'Expense'" />
        <BalanceInfo 
            :amount='20'
            :amountLabel = "'Income'" />
    </div>
</template>

<script>

import BalanceInfo from './BalanceInfo.vue';

export default {
    name : 'MainBoard',
    components : {
        BalanceInfo
    }
}
</script>

<style scoped>

.container{
    display: flex;
}
</style>