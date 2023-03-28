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
    <div class="container">
        Risultati trovati: {{ store.cardsFound }}
    </div>
</template>

<style lang="scss" scoped>
.container{
    background-color: #212529;
    color: white;
    padding: 15px;
}

</style>

