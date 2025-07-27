<script setup lang="ts">
defineProps<{
  name: string;
}>();
</script>

<template>
  <div>
    <span class="material-symbols-outlined">{{ name }}</span>
  </div>
</template>
