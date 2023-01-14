<script setup lang='ts'>
import { ref, computed } from 'vue'
import NumPad from './components/NumPad.vue'

const word = ref([['a']])

function add(chars:string[]) {
    word.value.push(chars)
}

const combos = computed(() => {
    word.value.forEach()
    return word.value
})

//function getCombos(pre, current, remaining)
</script>


<template>
<div>
    {{ JSON.stringify(word) }}
    {{ JSON.stringify(combos) }}
    <NumPad @clicked='add'/>
</div>
</template>


<style scoped>

</style>
