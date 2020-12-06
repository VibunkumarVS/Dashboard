<template>
    <div class="container">
        <div class="amount_field">₹ {{ amount }}</div>
        <div class="amount_label">{{ amountLabel }}</div>
    </div>
</template>

<script>
export default {
    name: 'BalanceInfo',
    props: {
        amount :{
            type: Number
        },
        amountLabel :{
            type: String
        }
    }
}
</script>

<style scoped>

.container{
    margin: 0 5px;
    display: flex;
    flex-direction: column;
    width: 100px;
    text-align: right;
}

.amount_field{
    font-size: 25px;
    font-weight: bold;
}

.amount_label{
    font-size: 13px;
}

</style>