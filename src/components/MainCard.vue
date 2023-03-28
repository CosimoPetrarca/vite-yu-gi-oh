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
    <div class="card text-center">
        <img :src="img">
        <h5>{{ name }}</h5>
        <div>{{ type }}</div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: 100%;
    background-color: orange;
    margin-bottom: 20px;

    h5 {
        color: white;
        padding-top: 20px;
    }
}
</style>