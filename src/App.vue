<template>
  <div id="app">

    <appHeader :quotes='quotes' :maxQuotes="maxQuotes"></appHeader>
    <newQuote> </newQuote>
      
    
  </div>
</template>

<script>
import header from './components/Header.vue';
import newQuote from './components/newQuote.vue';

export default {
  name: 'app',
  data: function () {
            return {
                quotes: [
                    'Just a Quote to see something'
                ],
                maxQuotes: 100
            }
        },
        methods: {

        },
        components: {

            appHeader: header,
            newQuote: newQuote,
        }
}
</script>

<style lang="scss">

</style>
