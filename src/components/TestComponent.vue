<template>
  <div class="card">
    <button type="button" @click="increaseCountAndLog">count is {{ count }}</button>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'



const count = ref(0)

function increaseCountAndLog() {
  count.value++

  console.log('hey, you just clicked me')
}
</script>