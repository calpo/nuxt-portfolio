<template>
    <div class="pnWrapper">
        <NuxtLink :to="前の記事へのリンク">
            <img src="~/assets/images/arrow-left.svg" alt="arrow-left" />
            <h3>前の記事のタイトル</h3>
        </NuxtLink>
        <NuxtLink :to="次の記事へのリンク">
            <h3>次の記事のタイトル</h3>
            <img src="~/assets/images/arrow-right.svg" alt="arrow-right" />
        </NuxtLink>
    </div>
</template>