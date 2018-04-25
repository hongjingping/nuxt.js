<template>
  <div>
    <h2>news Index page</h2>
    <p>newsId:{{$route.params.newsId}}</p>
    <ul>
      <li><nuxt-link :to="{name: 'news'}">News</nuxt-link></li>
      <li><nuxt-link :to="{name: 'news-id', params: {id: 123, title: 'I am wikiHong'}}">News-1</nuxt-link></li>
      <li><nuxt-link :to="{name: 'news-id', params: {id: 456}}">News-2</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>

</style>
