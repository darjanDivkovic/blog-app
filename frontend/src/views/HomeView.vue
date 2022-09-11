<template>
  <div class="home">
    <div class="home__content">
      <h1 class='home__header'>The Blog</h1>
      <Article/>

    </div>
  </div>
</template>

<script>
import Article from '@/components/Article'
export default {
  name: 'HomeView',
  components: {
    Article
  }
}
</script>

<style lang="sass" scoped>
.home
  border-radius: 5px
  background: #E5E6ED
  margin: 3% 6% 0 6%
  height: 100vh
  overflow: hidden
  h1
    font-family: 'Poppins'
    font-size: 75px
    color: #131312
  &__content
    margin: 150px 12% 0 12%
    height: 100vh
</style>