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
        <h5>{{ name }}</h5>
        <div>{{ type }}</div>
    </article>
</template>


<style lang="scss" scoped>
img{
    width: 70%;
}
</style>