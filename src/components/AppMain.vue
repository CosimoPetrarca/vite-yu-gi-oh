<script>
import { store } from '../store';
import MainList from './MainList.vue';
import MainFound from './MainFound.vue';
export default {
    name: 'Main',
    components: {
        MainList,
        MainFound
    },

    data() {
        return {
            store
        }
    }
}
</script>

<template>
    <div>
        <div class="container">
            <form>
                <div class="row justify-content-start">
                    <div class="col-2 col-sm-auto">
                        <select name="type" id="selectType" class="mb-2" v-model="store.cardsArchetypesSelected"
                            @change="$emit('search')">
                            <option v-for="archetype in store.cardsArchetypes" :value="archetype.archetype_name">{{
                                archetype.archetype_name }}</option>
                        </select>
                    </div>
                </div>
            </form>
        </div>
        <div>
            <MainFound />
            <MainList />
        </div>
    </div>
</template>

<style lang="scss" scoped>
div {
    background-color: orange;

    select {
        margin: 30px 0;
        height: 35px;
        width: 150px;
    }
}
</style>