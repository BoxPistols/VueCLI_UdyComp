<template>
  <div class="l_block">
    <div class="">
      <like-head></like-head>
      <h2 class="totalNum"> {{ num }} </h2>
      <LikeNum :num="num"></LikeNum>
      <LikeNum :num="num"></LikeNum>
    </div>
  </div>
</template>

<script>
  // Local
  import LikeHead from "./assets/components/LikeHead";

  export default {
    data() {
      return {
        num: 12
      }
    },
    components: {
      LikeHead: LikeHead
    }
  }
</script>

<style lang="sass">
  .l_block
    background-color: lavender
    padding: 16px 32px 32px
  .totalNum
    font-size: 42px
    text-align: center
</style>
