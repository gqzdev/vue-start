<template>
  <section class="jumbotron">
    <h3 class="jumbotron-heading">Search Github Users</h3>
    <div>
      <form @click.prevent="search">
        <input type="text" placeholder="enter the name you search" v-model="searchName"/>
        <input type="submit" value="Search GitHub"/>
        <!--<button @click="search">Search</button>-->
      </form>
    </div>
  </section>
</template>

<script>
  import PubSub from 'pubsub-js'
  export default {
    data () {
      return {
        searchName: ''
      }
    },

    methods: {
      search () {
        const searchName = this.searchName.trim()
        if(searchName) {
          // 分发一个search的消息 (消息名，参数) [触发事件]
          PubSub.publish('search', searchName)
        }
      }
    }
  }
</script>

<style>

</style>
