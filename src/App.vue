<template>
  <div id="app">

    <div class="container">

      <appHeader :quotes='quotes' :maxQuotes="maxQuotes"></appHeader>
      <newQuote @quoteAdded="quoteAdded"> </newQuote>
      <quoteGrid :quotes='quotes'> </quoteGrid>

    </div>
      
    
  </div>
</template>

<script>
import header from './components/Header.vue';
import newQuote from './components/newQuote.vue';
import quoteGrid from './components/quoteGrid.vue';

export default {
  name: 'app',
  data: function () {
            return {
                quotes: [
                    'I wish I had done everything on earth with you. – F. Scott Fitzgerald.', 'For when the cold wind blows, I will close my eyes calmly, knowing I am anchored to you. – Tyler Knott Gregson.'
                ],
                maxQuotes: 100
            }
        },
        methods: {

            quoteAdded(quote){

              this.quotes.push(quote);
                

            },
        },

        components: {

            appHeader: header,
            newQuote: newQuote,
            quoteGrid: quoteGrid,
        }
}
</script>

<style lang="scss">

</style>
