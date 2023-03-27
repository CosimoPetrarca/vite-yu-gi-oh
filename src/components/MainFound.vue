<script>
import { store } from '../store';
export default {
    name: 'MainFound',
    data() {
        return {
            store
        }
    }
}
</script>

<template>
    <div>
        Risultati trovati: {{ store.cardsFound }}
    </div>
</template>

<style lang="scss" scoped>

</style>

