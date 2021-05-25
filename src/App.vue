<template>
  <div id="app">

    <app-header :maxQuotes="maxQuotes"></app-header>
      
    
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  name: 'app',
  data: function () {
            return {
                quotes: [
                    'Just a Quote to see something'
                ],
                maxQuotes: 10
            }
        },
        methods: {

        },
        components: {

            appHeader: Header
        }
}
</script>

<style lang="scss">

</style>
