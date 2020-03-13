<template>
    <nav class="nav">
        <div class="logo">
            <nuxt-link :to="{name: 'index'}" class="logo text-lg">
                Nuxt Tutorials
            </nuxt-link>
            <nuxt-link :to="{name: 'posts-id', params: {id: '1'}}">
                one
            </nuxt-link>

            <span class="subheader">
                A Vue School course
            </span>
        </div>
    </nav>
</template>

<script>
export default {
    
}
</script>

<style scoped>

</style>