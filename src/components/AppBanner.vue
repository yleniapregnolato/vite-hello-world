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
    <body>
        <div class="banner">
            <h2>{{ title }}</h2>

            <div class="cat"><img :src="getImagePath(image)" alt="" /></div>
        </div>
    </body>
</template>

<style>
body {
    display: flex;
    flex-direction: column;
}
h2 {
    text-align: center;
    margin-bottom: 20px;
}

img {
    padding: 30px;
}
.banner {
    background-color: lightblue;
}
.cat {
    display: flex;
    justify-content: center;
}
</style>