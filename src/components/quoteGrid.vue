<template>

                <div class="row">
                    <div class='quote_box' v-for="(quote, index) in quotes" >{{quote}}</div>
                </div>

</template>

<script>
   
    export default {
        props: ['quotes'],

        methods: {



        }
    }
</script>

<style>

    .quote_box {
        font-family: cursive;
        font-size: 24px;
        color: #6e6e6e;
    }

    .quote {
        cursor: pointer;
    }

    .quote:hover {
        background-color: #ffe2e2;
    }

</style>