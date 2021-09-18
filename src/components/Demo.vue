<!-- View -->
<template>
    <div>
        <h1>Style Scopes</h1>

        <p class="paragraph">A .paragraph class has style global</p>
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
.paragraph {
    background-color: lightgray;
}
</style>
