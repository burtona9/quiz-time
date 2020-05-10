<template>
<div>
    <p>{{questions}}</p>
    
</div>
</template>
<script>
export default {
    data: function(){
        return {
            questions = this.$store.questions
        }
    },
    methods:{
        onOptionSelected(){
            this.$emit("onOptionSelected");
        }
    }
}
</script>
<style>

</style>