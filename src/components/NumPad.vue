<script setup lang='ts'>
import NumButton from './NumButton.vue'
const emit = defineEmits(['clicked'])

const CHARS = [
    '', '',
    'abc',
    'def',
    'ghi',
    'jkl',
    'mno',
    'pqrs',
    'tuv',
    'wxyz'
]
</script>


<template>
<div class='border grid grid-cols-3 gap-3'>
    <NumButton
        v-for='n in 9'
        :key='n'
        :n='n'
        :chars="CHARS[n].split('')"
        @click="emit('clicked', CHARS[n].split(''))" />
</div>
</template>