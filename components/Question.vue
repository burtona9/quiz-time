<template>
<div>
    <p>{{question}}</p>
    <div v-for="(option,index) in options" :key="index" on:click="onOptionSelected">
        {{option.text}}
    </div>
</div>
</template>
<script>
export default {
    props:{
        question: String,
        options: Array
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
