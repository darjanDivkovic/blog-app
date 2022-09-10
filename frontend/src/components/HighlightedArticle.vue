<template>
<div class="highlighted-article-container">
<div class="section-left">
    <div class="section-img"></div>
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
    }

    .section-left {
        width:55%;
        border-radius: 5px;
        min-height: 350px;
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
        border-radius: 5px;
        background-image: linear-gradient(to right top, #f47173, #ef6783, #e46093, #d45ea3, #bf5fb2, #b35fbb, #a45fc3, #9261cb, #8b60d2, #835fda, #795ee1, #6c5ee9);
    }

    .section-right {
        text-align: left;
        padding-left: 40px;
    }

    .section-date {
        color: gray;
        font-size: 12px;
        padding-top: 10px;
    }

    .section-title {
        font-size: 45px;
        font-weight: 600;
        max-width: 80%;
        margin: 0;
    }

    .section-content {
        max-width: 80%;
        font-size: 14px;
        padding-bottom: 10px;
    }

    @media only screen and (max-width: 600px){
        .highlighted-article-container {
            flex-direction: column;
        }
        .section-left {
            width: 100%;
        }
    }

</style>