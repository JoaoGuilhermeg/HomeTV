<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/hometv.png' }
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
  img:'hometv.png' ,
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UHeader>
      <template #left>
        <img
        src="/hometv.png"
        alt="ìcone HomeTV"
        class="h-10 w-auto rounded-lg shadow-2xl rinr ring-default"
        >
        <TemplateMenu />
      </template>

     
    </UHeader>

    <UMain>
      <NuxtPage />
    </UMain>

    <USeparator icon="i-simple-icons-nuxtdotjs" />

    <UFooter>
      <template #left>
        <p class="text-sm text-muted">
          HomeTV • © {{ new Date().getFullYear() }}
        </p>
      </template>
      
    </UFooter>
  </UApp>
</template>
