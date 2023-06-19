<template>
    <div class="upperHeader">
        <img src="../assets/img/ygoLogo.png" alt="Yu-Gi-Oh logo">

        <h1>
            YU-GI-OH API
        </h1>
    </div>

    <div class="lowerHeader">

    </div>
</template>

<script>
    export default {
        name: "AppHeader",
    }
    </script>

<style lang="scss" scoped>

    div.upperHeader,
    div.lowerHeader{
        height: 70px;
    }
    div.upperHeader{
        display: flex;
        justify-content: start;
        align-items: center;

        img{
            height: 70px;
            padding: 0 1.5rem;
        }
    }

    div.lowerHeader{
        background-color: #D48F38;
    }
</style>