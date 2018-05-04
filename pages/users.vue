<template>
    <div class="formtest">
        <h2>Find a user</h2>
        <input type="text" v-model="userId"/>
        <button @click="onLoadUser">Load User Details</button>
        <nuxt-child/>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                userId: ''
            }
        },
        methods: {
            onLoadUser() {
                this.$router.push('/users/' + this.userId)
            }
        },
        name: "users"
    }
</script>

<style scoped>

</style>
