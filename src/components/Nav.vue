<template>
    <ul class="nav">
        <Item title="Home"/>
        <Item title="About Us"/>
        <Item title="Contact"/>
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
