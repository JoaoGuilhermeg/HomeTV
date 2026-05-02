<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/iconehometv.png' }
  ],
  htmlAttrs: {
    lang: 'pt-br'
  }
})

const title = 'HomeTV'
const description = 'A production-ready starter template powered by Nuxt UI. Build beautiful, accessible, and performant applications in minutes, not hours.'

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  img:'iconehometv.png',
  twitterCard: 'summary_large_image'
})
</script>

<template>
    <TemplateMenu />
    <uApp>
    <UMain>
      <NuxtPage />
    </UMain>

    <USeparator icon="iconehometv.png" />

    <UFooter>
      <template #left>
        <p class="text-sm text-muted">
          HomeTV • © {{ new Date().getFullYear() }}
        </p>
      </template>
      
    </UFooter>
  </UApp>
</template>
