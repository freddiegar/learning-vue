<!-- View -->
<template>
    <div>
        <h1>Hello {{ person.name }} {{ person.surname }}</h1>
        <!-- This is javascript -->
        <p>9 + 3 = {{ 9 + 3 }}</p>
        <p>{{ 'Con' + 'cat' }}</p>
        <p>{{ person.title }}</p>
        <p v-html="person.title"></p>
    </div>
</template>

<!-- Controller -->
<script>
    export default {
        name: 'Demo',
        data () {
            return {
                person: {
                    name: "Freddie",
                    surname: "Gar",
                    title: "<strike>Developer</strike>"
                }
            }
        }
    }
</script>

<!-- Styles -->
<style>

</style>
