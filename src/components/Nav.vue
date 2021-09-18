<template>
    <ul class="nav">
        <Item v-bind:dataItem="{ title:'Home', url:'/home' }" />
        <Item v-bind:dataItem="{ title:'About Us', url:'/about-us' }" />
        <Item v-bind:dataItem="{ title:'Contact', url:'/contact' }" />
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
        }
    },
}
</script>
