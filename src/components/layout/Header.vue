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
  <header id="header" class="w-full max-w-7xl h-20">
    <nav id="menu" class="flex flex-row justify-around items-center h-20">
      <h1 id="title" class="font-bold tracking-wider px-10">VICOMMERCE</h1>
      <ul id="list" class="flex flex-row w-80 max-w-sm justify-center">
        <li v-for="{ id, name } in menu" :key="id" class="px-5">{{ name }}</li>
      </ul>
      <div class="w-32 max-w-xs flex flex-row justify-evenly">
        <Icon name="person" />
        <Icon name="shopping_cart" />
      </div>
    </nav>
  </header>
</template>

<style>
#header {
  box-shadow:
    rgba(240, 46, 170, 0.4) 0px 5px,
    rgba(240, 46, 170, 0.3) 0px 10px,
    rgba(240, 46, 170, 0.2) 0px 15px,
    rgba(240, 46, 170, 0.1) 0px 20px,
    rgba(240, 46, 170, 0.05) 0px 25px;
}
</style>
