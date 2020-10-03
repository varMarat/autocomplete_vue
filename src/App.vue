<template>
  <div class="wrapper">
    <HeadTop />
    <HeadMid />
  </div>
</template>

<script>
import HeadTop from './components/HeadTop'
import HeadMid from './components/HeadMid'
export default {
  name: 'App',
  components:{HeadTop, HeadMid}

}
</script>

<style lang="scss">
  .wrapper{
    width: 100%;
    height: 100vh;
    margin: 0 auto;
  }
  .www{
    background: #FAFBFC;
  }
</style>
