<script setup>
import { defineProps } from 'vue'
const props = defineProps(['itemText'])
console.log(props.itemText)
</script>
<template>
  <span class="relative px-2 py-1 text-xl">
    <span class="group-hover:font-bold">{{ itemText }}</span>
    <div
      class="absolute left-0 top-0 hidden h-2 w-2 border-l-[1px] border-t-[1px] border-solid border-[#919191] group-hover:block"
    ></div>
    <div
      class="absolute right-0 top-0 hidden h-2 w-2 border-r-[1px] border-t-[1px] border-solid border-[#919191] group-hover:block"
    ></div>
    <div
      class="absolute bottom-0 left-0 hidden h-2 w-2 border-b-[1px] border-l-[1px] border-solid border-[#919191] group-hover:block"
    ></div>
    <div
      class="absolute bottom-0 right-0 hidden h-2 w-2 border-b-[1px] border-r-[1px] border-solid border-[#919191] group-hover:block"
    ></div>
  </span>
</template>
