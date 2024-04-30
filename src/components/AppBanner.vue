<script>
export default {
    data() {
        return {
           title: "gattino",
           image: "gattino.jpeg"
        };
    },
    methods: {
        getImagePath(imageName) {
            return new URL(`../assets/img/${imageName}`, import.meta.url).href;
        },
    },
};
</script>

<template>
    <div class="banner">
        <h2>{{ title }}</h2>
        <img :src="getImagePath(image)" alt="" />
    </div>
</template>

<style>
</style>