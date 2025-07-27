<script setup lang="ts">
import Icon from "../Icon.vue";

import type { item } from "@/interfaces";

const menu: item[] = [
  { id: 1, name: "promo" },
  { id: 2, name: "categoria" },
  { id: 3, name: "marcas" },
];
</script>

<template>
  <header id="header" class="w-full max-w-7xl">
    <nav id="menu" class="flex flex-row justify-around items-center h-20">
      <h1 id="title" class="font-bold tracking-wider">VICOMMERCE</h1>
      <ul id="list" class="flex flex-row">
        <li v-for="{ id, name } in menu" :key="id" class="px-5">{{ name }}</li>
      </ul>
      <Icon name="person" />
    </nav>
  </header>
</template>
