<template>
  <div class="space-y-6">
    <h2 class="shine text-4xl leading-snug text-zinc-50">
      <b>Merhaba, ben Zeynel</b>
    </h2>
    <div class="prose prose-xl">
      <p><a class="link" href="https://tesodev.com/">Tesodev</a>'de Frontend Developer olarak çalışmaktayım.</p>
      <p>
        Bu blogda, web teknolojileri hakkında bilgi ve deneyimlerimi sade ve anlaşılır şekilde aktarmayı hedefliyorum.
      </p>
      <p>Soru ve geri bildirimlerinizi bekliyor olacağım.</p>
    </div>
    <div class="flex items-center gap-2">
      <BaseSocial v-for="social in socials" v-bind="social">
        <span v-if="social.text" class="text-zinc-50 font-semibold mx-2">{{ social.text }}</span>
      </BaseSocial>
    </div>
  </div>
</template>

<script setup lang="ts">
// imports
import socials from "@/constants/socials";
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
