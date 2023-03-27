<script>
import { store } from '../store';
import MainCard from './MainCard.vue';
export default {
    name: 'MainList',
    components: {
        MainCard
    },
    data() {
        return {
            store
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div v-for="(card, index) in store.cards" class="col-2">
                <template v-if="index < 100">
                    <MainCard :img="card.card_images[0].image_url" :name="card.name" :type="card.type" />
                </template>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped></style>