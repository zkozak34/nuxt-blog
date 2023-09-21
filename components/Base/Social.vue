<template>
  <a
    :href="link"
    :target="target"
    class="p-3 bg-zinc-700 rounded-full flex items-center justify-center transition-all cursor-pointer"
    :class="wrapperClass"
  >
    <Icon v-if="icon" :name="icon" class="text-2xl text-zinc-50" :class="iconClass" />
    <template v-else><slot /></template>
  </a>
</template>

<script setup lang="ts">
// imports

// interfaces & types
interface IProps {
  key?: string;
  link: string;
  icon?: string;
  target?: string;
  wrapperClass?: string;
  iconClass?: string;
}
// constants

// composable

// props
withDefaults(defineProps<IProps>(), {
  wrapperClass: "hover:bg-indigo-900",
  target: "_black",
});
// defineEmits

// states (refs and reactives)

// computed

// watchers

// lifecycles

// methods
</script>

<style lang="postcss" scoped></style>
