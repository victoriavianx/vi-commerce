<script setup lang="ts">
defineProps<{
  name: string;
  customStyle?: string;
}>();
</script>

<template>
  <div :class="customStyle">
    <span class="material-symbols-outlined">{{ name }}</span>
  </div>
</template>
