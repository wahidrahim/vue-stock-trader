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
    data() {
        return {
            stocks: [
                {id: 1, name: 'Tesla', price: 353 },
                {id: 2, name: 'Google', price: 1005 },
                {id: 3, name: 'Twitter', price: 18 },
                {id: 4, name: 'Apple', price: 154 },
                {id: 5, name: 'Nike', price: 53 }
            ]
        }
    }
}
</script>

<style lang="css">
</style>
