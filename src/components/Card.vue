<template>
    <div class="card">
        <div class="card-body">
            <h5 class="card-title">
                {{ dataCard.title }}
            </h5>

            <p class="card-text">
                {{ dataCard.text }}
            </p>

            <Button />
        </div>
    </div>
</template>

<script>
import Button from './Button.vue'

export default {
    name: 'Card',
    components: {
        Button
    },
    data() {
        return {
        }
    },
    props: {
        dataCard: Object
    }
}
</script>
