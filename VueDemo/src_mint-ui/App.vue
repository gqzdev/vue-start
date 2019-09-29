<template>
  <mt-button type="primary" @click.native="handleClick" id="buttonTest">Test</mt-button>
</template>

<script>
  import { Toast } from 'mint-ui'

  export default {
    methods: {
      handleClick () {
        Toast('提示信息')
      }
    }
  }
</script>

<style>
  #buttonTest{
    width: 100%;
  }
</style>
