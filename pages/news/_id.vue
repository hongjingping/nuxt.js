<template>
  <div>
    <h2>news-content</h2>
    <p>newsId: {{ $route.params.id }}</p>
    <ul>
      <li><a href="/">Home</a></li>
    </ul>
  </div>
</template>

<script>
  export default {
    // 校验参数，如果id是非数字就进入nuxt404页面
    validate ({params}) {
      return /^\d+$/.test(params.id)
    },
    data () {
      return {
        title: this.$route.params.title
      }
    },
    head () {
      return {
        title: this.title,
        meta: [
          {hid: 'description', name: 'news1', content: 'this is news page'}
        ]
      }
    }
  }
</script>

<style scoped>

</style>
