<template>
    <div>
        <div class="cardWrapper">
            <SingleCard v-for="num in 20"/>
        </div>
    </div>
</template>

<script>
import SingleCard from './SingleCard.vue';

export default {

    name: 'CardsList',
    components: {
        SingleCard,
    }
}
</script>

<style lang="scss" scoped>
    div.cardWrapper{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
</style>