<template>
    <div class="wrapper">
        <div class="container">
            <h1>ブログページ</h1>
            <div v-for="entry in data" :key="entry.id">
                <div class="textsContainer">
                    <h3>{{ entry.title }}</h3>
                    <p>{{ entry.excerpt }}</p>
                    <p>{{ entry.date }}</p>
                    <NuxtLink :to="entry._path">Read more</NuxtLink>
                </div>
                <div class="blogImg">
                    <img :src="entry.image" alt="blog-image" style="width:300px; height:80px;">
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const { data } = await useAsyncData('blogQuery', () =>
    queryContent("/blog").sort({id:-1}).find()
)
</script>

<style>
h1 {
    color: red
}

.text {
    color: green;
    letter-spacing: 20px;
}
</style>