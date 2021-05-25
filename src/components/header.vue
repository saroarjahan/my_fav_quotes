<template>
    <div class="row">
        <div class="col-sm-12" >
            {{quotes}}
        </div>
    </div>
</template>
<script>
    export default {
        props: ['quotes', 'maxQuotes']
    }
</script>