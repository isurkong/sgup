<template>
    <h1>{{props.msg}}</h1>
    <button>click me</button>
</template>


<script setup lang="ts">
    const ENV = import.meta.env
    console.log('env:',ENV)
    const props = defineProps({
        msg: {
            type: String,
            default: ()=>'我是home组件',
        }
    })
</script>