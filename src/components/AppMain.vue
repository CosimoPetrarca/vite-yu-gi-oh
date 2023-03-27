<script>
import MainSearch from './MainSearch.vue';
import MainList from './MainList.vue';
import MainFound from './MainFound.vue';
export default {
    name: 'Main',
    components: {
        MainSearch,
        MainList,
        MainFound
    }
}
</script>

<template>
   <div>
        <MainSearch />
        <MainFound />
        <MainList />
    </div>
</template>



<style lang="scss" scoped>
</style>