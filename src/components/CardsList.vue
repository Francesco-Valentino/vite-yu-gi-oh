<template>
    <div>
        <div class="cardWrapper">
            <SingleCard v-for="card in cardsList"
                :cardName="card.name"
                :cardArchetype="card.archetype"
                :cardImage="card.card_images[0].image_url"
            />
        </div>
    </div>
</template>

<script>
import SingleCard from './SingleCard.vue';
import axios from 'axios';

export default {

    name: 'CardsList',
    components: {
        SingleCard,
    },

    data(){
        return{
            cardsList: [],
        }
    },

    created() {
        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0')
        .then((response) => {
            console.log(response.data.data);
            this.cardsList = response.data.data;
        })
    },
}
</script>

<style lang="scss" scoped>
    div.cardWrapper{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
</style>