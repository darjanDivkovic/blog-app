<template>
<div class='container'>
    <Article v-for="n in count" :key="n"/>
</div>
</template>

<script>
import Article from '@/components/Article.vue'

export default {
    name: 'ArticleGrid',
    components: {
        Article
    },
    data() {
        return {
            count: 6,
        }
    }
}
</script>

<style lang='sass' scoped>
.container
    margin-top: 50px
    display: grid
    grid-template-columns: 1fr 1fr 1fr
    column-gap: 5%
</style>