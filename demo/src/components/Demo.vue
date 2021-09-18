<!-- View -->
<template>
    <div>
        <h1>Hello {{ person.name }} {{ person.surname }}</h1>
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
                    surname: "Gar"
                }
            }
        }
    }
</script>

<!-- Styles -->
<style>

</style>
