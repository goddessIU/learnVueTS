<script setup lang="ts">
import { ref } from 'vue';

const name = ref<string>('Link')
const age = ref<string | number>(25)

const changeName = (val: string) => {
  name.value = val
}

const changeAge = (val: number | string) => {
  age.value = val
}
</script>

<template>
  <div class="app">
    <p>{{ name }} - {{ age }}</p>
    <button @click="changeName('sb')">change Name</button>
    <button @click="changeAge('30')">change Age</button>
  </div>
</template>

<style>

</style>
