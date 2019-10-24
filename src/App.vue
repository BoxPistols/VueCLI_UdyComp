<template>
  <div class="l_block">
    <div class="">
      <like-head></like-head>
      <LikeNum></LikeNum>
    </div>
  </div>
</template>

<script>
  // Local
  import LikeHead from "./assets/components/LikeHead";

  export default {
    // Local
    components: {
      LikeHead: LikeHead
    }
  }
</script>

<style lang="sass" >
  body
    padding: 2%
    .l_block
      max-width: 960px
      margin: auto
</style>
