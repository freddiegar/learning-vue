<!-- View -->
<template>
    <div>
        <h1>Conditionals</h1>

        <p v-if="persons[Math.floor(Math.random() * persons.length)].name !== 'Freddie'">
            Hello!
        </p>
        <p v-else-if="(Math.random() * 10).toFixed() % 3 === 0">
            You have luck, see you later!
        </p>
        <p v-else>
            Bye!
        </p>
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
                    },
                    {
                        name: "Jon",
                        surname: "Doe",
                        title: "<strike>QA</strike>"
                    },
                    {
                        name: "Jone",
                        surname: "Doe",
                        title: "<strike>Manager</strike>"
                    }
                ]
            }
        }
    }
</script>

<!-- Styles -->
<style>

</style>
