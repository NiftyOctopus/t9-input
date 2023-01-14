<script setup lang='ts'>
defineProps<{ n:number, chars:string[] }>()
</script>


<template>
<div class='border'>
    <div>{{ n }}</div>
    <div>{{ chars.join(' ') }}</div>
</div>
</template>