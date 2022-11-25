<template>
    <footer>
        <div class="insideContainer">
            <a href="https://www.google.com/"><img src="~/assets/images/github.svg" alt="github"></a>
            <a href="https://www.google.com/"><img src="~/assets/images/linkedin.svg" alt="linkedin"></a>
            <a href="https://www.google.com/"><img src="~/assets/images/twitter.svg" alt="twitter"></a>
            <a href="https://www.google.com/"><img src="~/assets/images/facebook.svg" alt="facebook"></a>
            <hr />
            <NuxtLink to="/blog">Blog</NuxtLink>
            <NuxtLink to="/contact">Contact</NuxtLink>
            <p>(c){{ new Date().getFullYear() }} Abe Hiroki</p>
        </div>
    </footer>
</template>