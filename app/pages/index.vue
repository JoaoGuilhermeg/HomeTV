<script setup lang="ts">
import type { ButtonProps } from '@nuxt/ui';


const links = ref<ButtonProps[]>([
  {
    label: 'Veja o catálogo',
    to:'',
    icon:'i-lucide-play',
    color:'primary' as const
  },
  {
    label:'Saiba mais.',
    to:'',
    color:'neutral' as const,
    variant:'subtle',
    trailingIcon:'i-lucide-arrow-right'
  }  
])
const items = [
  'iconehometv.png',
  'iconehometv.png',
  'iconehometv.png',
  'iconehometv.png'

]
</script>

<template>
<UContainer>
 <div class="grid grid-cols-2 gap-4 items-center">
 <UPageHero
    title="HomeTV"
    description="O lar dos melhores filmes você só encontra aqui! Acompanhe no nosso catálogo para ver as sinopses do filme que você procura."
    headline="Seja bem-vindo!"
    orientation="horizontal"
    :links="links"
  />
    <UCarousel
      v-slot="{ item }" 
      loop
      arrows
      :autoplay="{delay:1900 }"
      wheel-gestures
      :prev="{variant: 'solid' }"
      :next="{ variant: 'solid' }"
      :items="items"

      :ui="{
        item: 'basis-1/3 ps-0',
        prev: 'sm: start-8',
        next: 'sm: end-8',
        container: 'ms-0'
        }"
        class="w-full nax-w-xs mx-auto"
    >
      <img :src="item" width="320" height="320" class="rounded-lg" loading="lazy">
    </UCarousel>
    </div>
  </UContainer>
</template>

