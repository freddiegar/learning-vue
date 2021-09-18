<template>
    <button class="btn btn-primary" v-on:click="buttonClick(dataButton.label)">
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
    props: {
        dataButton: Object
    },
    methods: {
        buttonClick: function (label) {
            this.label = label;
        }
    }
}
</script>
