<!-- View -->
<template>
    <div>
        <h1>Hello {{ persons[0].name }} {{ persons[0].surname }}</h1>
        <!-- This is javascript -->
        <p>9 + 3 = {{ 9 + 3 }}</p>
        <p>{{ 'Con' + 'cat' }}</p>
        <p>{{ persons[0].title }}</p>
        <p v-html="persons[0].title"></p>
    </div>
</template>

<!-- Controller -->
<script>
    export default {
        name: 'Demo',
        data () {
            return {
                persons: [
                    {
                        name: "Freddie",
                        surname: "Gar",
                        title: "<strike>Developer</strike>"
                    }
                ]
            }
        }
    }
</script>

<!-- Styles -->
<style>

</style>
