<script setup lang="ts">
defineProps<{
  variant?: string;
}>();
</script>

<template>
  <button
    class="bg-red-400 text-white border-black border-2 pop-out rounded-lg p-2 active:bg-green-300 active:text-black hover:-translate-x-1 hover:-translate-y-1 transition-all"
  >
    <slot></slot>
  </button>
</template>

<style scoped>
.pop-out:hover {
  box-shadow:
    1px 1px black,
    2px 2px black,
    3px 3px black,
    4px 4px black;
}

.pop-out:active {
  box-shadow:
    1px 1px black,
    2px 2px black;
  transform: translate(-2px, -2px);
}
</style>
