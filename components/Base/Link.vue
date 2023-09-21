<template>
  <span class="rounded-md group">
    <nuxt-link
      :to="to"
      :class="customClass"
      class="transition-all group-hover:text-gray-100"
      exact-active-class="text-gray-100"
      ><slot
    /></nuxt-link>
  </span>
</template>

<script setup lang="ts">
// imports

// interfaces & types
interface IProps {
  to: string;
  customClass?: string;
}
// constants

// composable

// props
defineProps<IProps>();
// defineEmits

// states (refs and reactives)

// computed

// watchers

// lifecycles

// methods
</script>

<style lang="postcss" scoped></style>
