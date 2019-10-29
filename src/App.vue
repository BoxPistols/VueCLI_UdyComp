<template>
  <div class="l_block">
    
    <div class="">
      
      <like-head></like-head>
      
      <!-- <h2 class="totalNum"> {{ num / 2 }} </h2> -->
      <like-num :num="num"></like-num>
      <like-num :num="num"></like-num>
    
    </div>

  </div>
</template>

<script>
  // Local
  import LikeHead from "./assets/components/LikeHead";

  export default {
    data() {
      return {
        num: 0
      }
    },
    components: {
      LikeHead
    }
  };
</script>

<style lang="sass">
  .l_block
    background-color: lavender
    padding: 16px 32px 32px
  .totalNum
    font-size: 42px
    text-align: center
</style>
