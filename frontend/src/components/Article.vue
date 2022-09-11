<template>
<div class="container" :class="{mini: isMini}">
    <div class="container__left" :class="{mini: isMini}">
        <div class="img" :class="{mini: isMini}"></div>
    </div>
    <div class="container__right">
        <span class="date">September 10. 2022</span>
        <span class="title" :class="{mini: isMini}">Tentang Creativity block pada UI Designer</span>
        <span class="content">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</span>
    </div>
</div>
</template>

<script>
export default {
    name: 'Article',
    props: ['isMini'],
}
</script>

<style lang="sass" scoped>
.container
  display: flex
  flex-direction: row
  &.mini
    display: flex
    border: 1px solid red
    flex-direction: column
  &__left
    width:55%
    border-radius: 5px
    min-height: 350px
    &.mini
        height: 175px
    .img
      height: 100%
      width:100%
      border-radius: 5px
      background-image: linear-gradient(to right top, #f47173, #ef6783, #e46093, #d45ea3, #bf5fb2, #b35fbb, #a45fc3, #9261cb, #8b60d2, #835fda, #795ee1, #6c5ee9)
      &.mini
        height: 50%
  &__right
    width:40%
    display: flex
    flex-direction: column
    justify-content: space-between
    padding-left: 40px
    &.mini
      width: 100%
    .date
      color: gray
      font-size: 12px
      padding-top: 10px
    .title
      font-size: 45px
      font-weight: 600
      max-width: 80%
      margin: 0
    .content
      max-width: 80%
      font-size: 14px
      padding-bottom: 10px

  @media (max-width: 600px) 
  .container 
    flex-direction: column
    &__left 
      width: 100%
</style>
