<template>
  <div id="app">

    <div v-for="item in quotes"> {{item}}</div>


    
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      quotes: ['my first quotes']
    }
  }
}
</script>

<style lang="scss">

</style>
