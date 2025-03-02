<script setup lang="ts">
import type { MenuItem } from "./interface";

const menuList: MenuItem[] = [
  { id: 1, name: "promo", path: "/" },
  { id: 2, name: "categoria", path: "/" },
  { id: 1, name: "marcas", path: "/" }
];
</script>

<template>
  <div id="header" class="h-16 flex flex-row w-full justify-center items-center">
    <h1>Vicommerce</h1>
    <nav>
      <ul class="flex flex-row justify-between">
        <li v-for="{ id, name } in menuList" :key="id">
          {{ name }}
        </li>
      </ul>
    </nav>
  </div>
</template>
