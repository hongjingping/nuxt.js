<template>
  <section class="container">
    <div>
      <div class="dist">
        <!-- <img src="~assets/images/location.png" alt=""> -->
      </div>
      <ul>
        <li><nuxt-link :to="{name: 'index'}">Home</nuxt-link></li>
        <li><nuxt-link :to="{name: 'about'}">About</nuxt-link></li>
        <li><nuxt-link :to="{name: 'news', params: {newsId: '1108'}}">News</nuxt-link></li>
        <li><nuxt-link :to="{name: 'asyncData'}">asyncData</nuxt-link></li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.dist {
  width: 100%;
  height: 300px;
  background-image: url('~assets/images/location.png');
}
</style>
