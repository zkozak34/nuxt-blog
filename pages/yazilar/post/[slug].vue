<template>
  <ContentRenderer :value="data!">
    <div class="prose">
      <h1>{{ data!.title }}</h1>
      <!-- <div class="border-b border-solid border-zinc-600"></div> -->
      <ContentRendererMarkdown :value="data!" />
    </div>
  </ContentRenderer>
  <!-- <pre>{{ data }}</pre> -->
</template>

<script setup lang="ts">
// imports

// interfaces & types

// constants

// composable
const route = useRoute();
const { data } = await useAsyncData("post", () => queryContent("/posts").where({ slug: route.params.slug }).findOne());
// props

// defineEmits

// states (refs and reactives)

// computed

// watchers

// lifecycles

// methods
</script>

<style lang="postcss" scoped></style>
