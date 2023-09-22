<template>
  <div>
    <h2 class="text-2xl font-bold text-white">Yazılar</h2>
    <div class="border-b border-solid border-zinc-600" />
    <div class="my-4 flex flex-col gap-6">
      <div v-for="post in data" class="flex flex-col gap-4 w-full">
        <h3 class="text-xl font-semibold text-zinc-200">
          <a :href="'/yazilar/post/' + post.slug">{{ post.title }}</a>
        </h3>
        <p class="line-clamp-2">{{ post.description }}</p>
        <span class="ml-auto text-xs italic text-zinc-400">{{ post.author }} ~ {{ post.date }}</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
// imports

// interfaces & types
interface IPost {
  title: string;
  description: string;
}
// constants

// composable
const { data } = await useAsyncData("posts", () => queryContent("/posts").find());
// props

// defineEmits

// states (refs and reactives)

// computed

// watchers

// lifecycles

// methods
</script>

<style lang="postcss" scoped></style>
