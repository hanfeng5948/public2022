<template>
    <div class="hello">Hello {{who}},is{{unitid}}</div>
</template>
 
<script>
module.exports = {
    data: function() {
        return {
            who: 'world'
        }
    },
    props:{unitid:Number}
}
</script>
 
<style>
.hello {
    background-color: #ffe;
}
</style>