<template lang="html">
    <div class="home">
        <h1>Trade &amp; View your Portfolio</h1>
        <h4>You may Save &amp; Load your data</h4>
        <h4>Click 'End Day' to begin a new day</h4>
        <hr>
        <p>Your funds: {{ funds | currency }}</p>
    </div>
</template>

<script>
export default {
    computed: {
        funds() {
            return this.$store.getters.funds
        }
    }
}
</script>

<style lang="css">
</style>
