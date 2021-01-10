<template>
<div class="container">

    <ListItem v-for="list in loadedlists" :key="list.id" 
        :description="list.description"
        :label="list.labels"
        :amount="list.amount"
        :type="list.type"
    />
</div>
</template>

<script>

import ListItem from './ListItem.vue';

export default {
    name: 'Lists',
    data(){
        return{
            loadedlists: [
            {
                id: 1,
                value: 'List',
                description: 'Spotifiy Sub',
                labels: 'Productivity',
                amount: '$ 2500',
                type: 'expense'
            },
            {
                id: 2,
                value: 'List 2',
                description: 'James Invoice',
                labels: 'Works',
                amount: '$ 2000',
                type: 'income'

            },
            {
                id: 3,
                value: 'List 3',
                description: 'UI8 Sales',
                labels: 'Micro Stock',
                amount: '$ 750',
                type: 'income'

            }
        ]
        }
        
    },
    components: {
        ListItem
    },
    created(){
        console.log("Lists comp created");
        this.loadlists();
    },
    methods: {
        loadlists(){
            console.log("loadlists ()");
        }
    }
}
</script>

<style scoped>

.container{
    margin-top: 40px;
    font-weight: 600;
    font-size: 14px;
}

</style>