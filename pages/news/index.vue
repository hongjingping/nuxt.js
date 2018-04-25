<template>
  <div>
    <h2>news Index page</h2>
    <p>newsId:{{$route.params.newsId}}</p>
    <ul>
      <li><a href="/">News</a></li>
      <li><a href="/news/123">News-1</a></li>
      <li><a href="/news/wikiHong">News-2</a></li>
    </ul>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>

</style>
