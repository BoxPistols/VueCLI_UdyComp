<template>
  <div class="container">
    <div class="row">
      <header>Head</header>
      <p>いいね（ {{ num }} ）</p>
    </div>
    <div class="row">
      <button class="button column column-25 column-offset-25" @click="inc"> +1 </button>
      <button class="button column column-25 column-offset-25" @click="reset"> reaet </button>
    </div>
  </div>
</template>

<script>
  export default {
    data: function () {
      return {
        num: 5
      }
    },
    methods: {
      inc: function () {
        this.num += 1
      },
      reset: function () {
        this.num = 0
      }
    }
  }
</script>

<style scoped lang="sass">
  div
    text-align: center
</style>
