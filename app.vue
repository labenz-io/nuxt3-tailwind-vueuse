<template>
  <h1 ref="header" class="text-3xl font-bold underline">{{ st }}</h1>
</template>

<script setup>
const st = ref('hello world')

const { width, height } = useWindowSize()

onMounted(() => {
  console.log(width.value, height.value)
})
</script>
