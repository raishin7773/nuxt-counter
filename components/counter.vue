<template>
  <section>
    <h2>{{title}}</h2>
    counter:{{$store.state.counter.counter}}
    <button v-on:click="$store.commit('counter/countUp')">+1</button>
    <button v-on:click="$store.commit('counter/reset')">reset</button>
  </section>
</template>

<script>
export default {
  name: "counter.vue",
  data: function () {
    return {
      title:'counter app'
    }
  }
}
</script>

<style scoped>

</style>
