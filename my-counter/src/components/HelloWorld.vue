<template>
  <div class="hello">
    <button v-on:click="addHandle">+</button>
    <button v-on:click="minusHandle">-</button>
    <span>{{ num }}</span>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      num: 0
    }
  },
  methods: {
    addHandle: function () {
      this.num++;
    },
    minusHandle: function () {
      this.num--;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
