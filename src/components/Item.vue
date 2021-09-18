<template>
    <li class="nav-item" v-bind:class="{ active: dataItem.current }">
        <a class="nav-link" v-bind:style="{ color: randomColor }" v-bind:href="dataItem.url">{{ dataItem.title }}</a>
    </li>
</template>

<script>
export default {
    name: 'Item',
    data() {
        return {
            randomColor: '#' + (Math.floor(Math.random() * 6777215)).toString(16)
        }
    },
    props: {
        dataItem: Object
    }
}
</script>
