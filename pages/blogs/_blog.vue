<template>
    <div>
     <h1>i am a blog post</h1>
    </div>
</template>

<script>
    export default {
        created() {
            console.log(this.$route.params)
        }
    }
</script>

<style lang="scss" scoped>

</style>