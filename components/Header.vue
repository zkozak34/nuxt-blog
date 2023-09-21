<template>
  <header class="py-4 flex items-center space-x-6">
    <BaseLink v-for="nav in navigation" :key="nav.key" :to="nav.to">{{ nav.text }}</BaseLink>
  </header>
</template>

<script setup lang="ts">
// imports
import navigation from "../constants/navigation";
// interfaces & types

// constants

// composable

// props

// defineEmits

// states (refs and reactives)

// computed

// watchers

// lifecycles

// methods
</script>

<style lang="postcss" scoped></style>
