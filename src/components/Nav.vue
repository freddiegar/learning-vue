<template>
    <ul class="nav">
        <Item v-bind:dataItem="item" v-for="(item, index) in items" :key="index" />
    </ul>
</template>

<script>
import Item from './Item.vue'

export default {
    name: 'Nav',
    components: {
        Item
    },
    data() {
        return {
            items: [
                { title:'Home', url:'/home', current: true },
                { title:'About Us', url:'/about-us' },
                { title:'Contact', url:'/contact' },
                { title:'Maps', url:'/maps' },
            ]
        }
    },
}
</script>
