<script setup lang="ts">
import BaseButton from './BaseButton.vue';
import TextInput from './TextInput.vue';
</script>

<template>
  <div class="border-black border-2 rounded-md bg-white p-4 grid gap-2 w-96">
    <p class="text-xl">Welcome : )</p>
    <form class="grid gap-4" @submit.prevent="">
      <label for="email" class="text-sm grid gap-1">Email<TextInput /></label>

      <BaseButton>Submit</BaseButton>
    </form>
  </div>
</template>
