<script>
    export default {
        name: 'MainCard',
        props: {
            img: String,
            name: String,
            type: String
        }

    }
</script>


<template>
    <article>   
        <div class="img"><img :src="img"></div>
        <h3>{{ name }}</h3>
        <div>{{ type }}</div>
    </article>
</template>


<style lang="scss" scoped>
</style>