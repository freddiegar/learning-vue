<template>
    <div class="card">
        <div class="card-body">
            <h5 class="card-title">
                {{ dataCard.title }}
            </h5>

            <p class="card-text">
                {{ dataCard.text }}
            </p>

            <p>
                What is your name: <input v-model="inputMessage" />
            </p>

            <p>
                {{ inputMessage }}!
            </p>
        </div>

        <div class="card-footer">
            <button class="btn btn-secondary mr-3"
                @click="inputMessage = 'Hi'"
                @mouseover="inputMessage = 'Welcome :D'"
                @mouseleave="inputMessage = 'Bye ;('"
                @dblclick="inputMessage = 'Surprise :0'"
                >
                I'm not a component
            </button>

            <Button v-bind:dataButton="{ label: 'Button 1' }" />

            <Button v-bind:dataButton="{ label: 'Button 2' }" />
        </div>
    </div>
</template>

<script>
import Button from './Button.vue'

export default {
    name: 'Card',
    components: {
        Button,
    },
    data() {
        return {
            inputMessage: 'Click any button'
        }
    },
    props: {
        dataCard: Object
    }
}
</script>
