<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <div class="hello-container">
    <h1>Hello World</h1>
  </div>
</template>

<style lang="postcss" scoped>
.hello-container {
  & > h1 {
    color: red;
  }
}
</style>
