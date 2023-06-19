<template>
    <main>
        <div class="container">
            <div>
                <CardsList />
            </div>
        </div>
    </main>
</template>

<script>
import CardsList from './CardsList.vue';

export default {
    name: 'AppMain',

    components: {
        CardsList,
    }
}
</script>

<style lang="scss" scoped>
    main{
        background-color: #D48F38;

        div.container{
            background-color: white;
        }
    }
</style>