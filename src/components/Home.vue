<template>
    <div>
        <h1>Trade or View your Portfolio</h1>
        <br>
        <h6>You may Save and Load your Data</h6>
        <h6>Click on 'End Day' to Begin a New Day!</h6>
        <hr>
        <p>Your Funds: {{funds | currency}}</p>
    </div>
</template>

<script>
export default {
    computed: {
        funds() {
            return this.$store.getters.funds;
        }
    }
}
</script>

