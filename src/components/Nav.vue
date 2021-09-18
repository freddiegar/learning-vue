<template>
    <ul class="nav">
        <li class="nav-item">
            <a class="nav-link" v-bind:class="{ active: isCurrent }" href="#">Home</a>
        </li>
        <li class="nav-item" v-bind:style="{ backgroundColor: randomColor }">
            <a class="nav-link" href="#">About Me</a>
        </li>
        <li class="nav-item" v-bind:style="{ backgroundColor: randomColorAlt, border: 'solid 3px' }">
            <a class="nav-link" href="#">Contact</a>
        </li>
        <li class="nav-item">
            <p class="paragraph">This .paragraph class has style scoped</p>
        </li>
    </ul>

</template>

<script>
export default {
    name: 'Nav',
    data() {
        return {
            isCurrent: (Math.random() * 10).toFixed() % 2 === 0,
            randomColor: '#' + (Math.floor(Math.random() * 6777215)).toString(16),
            randomColorAlt: '#' + (Math.floor(Math.random() * 6777215)).toString(16)
        }
    },
}
</script>

<style scoped>
.paragraph {
    background-color: gray;
}
</style>
