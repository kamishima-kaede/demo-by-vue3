<template>
  <div class="App">{{ store.count }}</div>
  <el-button type="primary" @click="add">+1</el-button>
</template>

<script setup>
import { reactive } from 'vue'
const store = reactive({
  count: 0
})
const add = () => {
  store.count++
}
</script>

<style scoped>
</style>