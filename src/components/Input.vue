<template>
    <!-- <input v-bind:value="dataInput ? dataInput.value : 'Empty'" /> -->
    <input v-bind:value="value" />
</template>

<script>
export default {
    name: 'Input',
    data() {
        return {
        }
    },
    props: {
        // dataInput: Object
        value: String
    }
}
</script>
