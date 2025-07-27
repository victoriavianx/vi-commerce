<script setup lang="ts">
defineProps<{
  title: string;
  options: { name: string }[];
}>();
</script>

<template>
  <v-menu open-on-hover transition="slide-x-transition">
    <template v-slot:activator="{ props }">
      <v-btn v-bind="props">{{ title }}</v-btn>
    </template>

    <v-list>
      <v-list-item v-for="(item, index) in options" :key="index" :value="index">
        <v-list-item-title>{{ item.name }}</v-list-item-title>
      </v-list-item>
    </v-list>
  </v-menu>
</template>
