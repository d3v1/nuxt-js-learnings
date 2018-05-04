<template>
    <h1>User ID is: {{ $route.params.id }}</h1>
</template>

<script>
    export default {
        validate(data) {
            return /^[0-9]+$/.test(data.params.id);
        }
    }
</script>

<style scoped>

</style>
