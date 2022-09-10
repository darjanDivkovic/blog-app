<template>
<div class="highlighted-article-container">
<div class="section-left">
    <img class="section-img" src="https://i.picsum.photos/id/718/536/354.jpg?hmac=h5RFx_Qwps-hOPBUGQzU3Kk9XXLJuvxbbWMEBCZYwPE" alt="lorem ipsum image">
</div>
<div class="section-right">
    <span class="section-date">September 10. 2022</span>
    <span class="section-title">Tentang Creativity block pada UI Designer</span>
    <span class="section-content">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</span>
</div>
</div>
</template>

<script>
export default {
    name: 'HighlightedArticle',
}
</script>

<style>
    .highlighted-article-container {
        display: flex;
        justify-content: center;
        height: 350px;
    }

    .section-left {
        width:55%;
        border: 1px solid #aab3c8;
        border-radius: 5px;
    }

    .section-right {
        width:40%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .section-img {
        height: 100%;
        width:100%;
    }

    .section-right {
        text-align: left;
        padding-left: 20px;
    }

    .section-date {
        color: gray;
        font-size: 12px;
        padding-top: 10px;
    }

    .section-title {
        font-size: 36px;
        font-weight: 600;
        max-width: 70%;
        margin: 0;
    }

    .section-content {
        max-width: 70%;
        font-size: 14px;
        padding-bottom: 10px;
    }

</style>