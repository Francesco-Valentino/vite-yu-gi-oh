<template>
    <div class="cardElement">
        <img :src="cardImage" :alt=" cardName + ' card proxy' ">
        
        <h4>
            {{ cardName }}
        </h4>

        <p>
            {{ cardArchetype }}
        </p>
    </div>
</template>

<script>
export default {
    name: "SingleCard",

    props: {
        cardName: String,
        cardArchetype: String,
        cardImage: String,
    },
}
</script>

<style lang="scss">
    div.cardElement{
        margin: .5rem 1rem;
        width: calc((100% / 5) - 2rem);
        text-align: center;
        height: 300px;
        display: flex;
        flex-direction: column;
        background-color: #D48F38;

        img{
            width: 100%;
        }

        h4{
            color: white;
        }

        p{
            color: rgb(79, 79, 79);
        }
    }
</style>