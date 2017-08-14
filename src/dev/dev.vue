<template>
  <aside class="dev">
    <label v-for="i in [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30]">
      测试数据{{i}}
      <br>
    </label>
    <VueBackTop :visibleOffset="visibleOffset" :className="'no-bar'"></VueBackTop>
  </aside>
</template>
<script>
  import VueBackTop from '../components/backTop.vue'
  export default {
    data() {
      return {
        visibleOffset: 400
      };
    },
    components: {VueBackTop}
  };
</script>
<style rel="stylesheet/scss" lang="scss">
  .dev {
    text-align: center;
    label {
      width: 7.5rem;
      height: 2rem;
      font-size: .28rem;
    }
  }


</style>

