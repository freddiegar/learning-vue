<template>
    <button class="btn btn-primary" v-on:click="buttonClick">
        {{ label }}
    </button>
</template>

<script>
export default {
    name: 'Button',
    data() {
        return {
            label: 'Click me!' // Default value
        }
    },
    methods: {
        buttonClick: function () {
            this.label = 'Click Event'
        }
    }
}
</script>
