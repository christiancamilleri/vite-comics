<script>
export default {
    data() {
        return {
            content: "--> Content goes here <--"
        }
    }
}
</script>

<template>
    <div class="container">
        {{ content }}
    </div>
</template>

<style lang="scss" scoped>
.container {
    padding: 90px 0;
}
</style>