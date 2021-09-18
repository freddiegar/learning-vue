<!-- View -->
<template>
    <div>
        <h1>Hide Elements</h1>

        <p>A paragraph is hidden using v-show</p>
        <p v-show="(Math.random() * 10).toFixed() % 2 === 0">
            Show paragraph
        </p>
    </div>
</template>

<!-- Controller -->
<script>
    export default {
        name: 'Demo',
        data () {
            return {
            }
        }
    }
</script>

<!-- Styles -->
<style>

</style>
