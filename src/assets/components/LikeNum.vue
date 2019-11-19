<template>
  <div class="container">
    <div class="row">
      <h3>いいね（ {{ num }} ）/ {{ halfNum }}</h3>
    </div>
    <div class="row">
      <button class="button column column-25 " @click="inc"> +1 </button>
      <button class="button column column-25 " @click="reset"> reaet </button>
    </div>
  </div>
</template>

<script>
  export default {
    // props: ["num"],
    props: {
      num: {
        type: Number,
        required: true

      }
    },

    computed: {
      halfNum() {
        return this.num + this.num;
      }
    },
    
    methods: {
      inc() {
        this.num += 1
      },
      reset() {
        this.num = 0
      }
    }
  };
</script>

<style scoped lang="sass">
.row
  justify-content: center
.button
  margin: 8px 8px 32px
p
  margin: 0
</style>
