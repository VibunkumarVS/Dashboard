<template>
    <div class="lineItem">
        <div class="description">{{ description }}</div>
        <div class="label">{{ label }}</div>
        <div class="amount"> {{amountSymbol}}  {{ amount }}</div>
    </div>    
</template>

<script>

export default {
    name: '',
    props: ['description', 'label', 'amount', 'type'],
    computed : {
        amountSymbol() {
            return this.type === "income" ? "+" : "-"
        }
    }
}

</script>

<style scoped>

.lineItem{
    width: 100%;
    margin: 20px 0;
    padding: 3px;
    display: flex;
}

.description{
    width: 50%;
}

.label{
    width: 25%;
}

.amount{
    width: 25%; 
    text-align: right;
}

</style>

