<template lang="html">
    <div class="stocks">
        <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
    </div>
</template>

<script>
import AppStock from './Stock.vue'
export default {
    components: {
        AppStock
    },
    computed: {
        stocks() {
            return this.$store.getters.stocks
        }
    }
}
</script>

<style lang="css">
</style>
