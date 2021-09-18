<template>
    <li class="nav-item" v-bind:class="{ active: isCurrent }" v-bind:style="{ backgroundColor: randomColor }">
        <a class="nav-link" href="#">{{ title }}</a>
    </li>
</template>

<script>
export default {
    name: 'Item',
    data() {
        return {
            isCurrent: (Math.random() * 10).toFixed() % 2 === 0,
            randomColor: '#' + (Math.floor(Math.random() * 6777215)).toString(16),
        }
    },
    props: {
        title: String
    }
}
</script>
