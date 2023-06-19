<template>
    <div>
        <h1>
            MAIN
        </h1>

        <div>
            <CardsList />
        </div>
    </div>
</template>

<script>
import CardsList from './CardsList.vue';

export default {
    name: "AppMain",

    components: {
        CardsList,
    }
}
</script>

<style lang="scss" scoped>
    
</style>