<!-- View -->
<template>
    <div>
        <h1>Loops</h1>

        <p>Simple</p>
        <ol>
            <li v-for="number in numbers" v-bind:key="number">{{ number }}</li>
        </ol>

        <p>Object</p>
        <ul>
            <li v-for="person in persons" v-bind:key="person">
                Name: {{ person.surname }}, {{ person.name }} |
                Title: {{ person.title }}
            </li>
        </ul>
    </div>
</template>

<!-- Controller -->
<script>
    export default {
        name: 'Demo',
        data () {
            return {
                numbers: [
                    'one',
                    'two',
                    'three'
                ],
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
