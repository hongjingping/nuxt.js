<template>
  <div>
    <h1>姓名:{{info.name}}</h1>
    <h1>年龄:{{info.age}}</h1>
    <h1>爱好:{{info.interast}}</h1>
    {{name}}
  </div>
</template>

<script>
  import axios from 'axios'
  export default {
    data () {
      return {
        name: 'Hello world, wikiHong'
      }
    },
    // promise方法
    // asyncData () {
    //   return axios.get('https://api.myjson.com/bins/smjj3')
    //   .then((res) => {
    //     return { info: res.data }
    //   })
    // },
    // await方法
    async asyncData () {
      let {data} = await axios.get('https://api.myjson.com/bins/smjj3')
      return {info: data}
    }
  }
</script>

<style scoped>

</style>
