<template>
<div>

    <ListItem v-for="list in loadedlists" :key="list.id" :defaultValue="list.value"/>
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
                value: 'Hello'
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