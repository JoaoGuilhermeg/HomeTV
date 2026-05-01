<script setup lang="ts">
import type { ButtonProps } from '@nuxt/ui';

const links = ref<ButtonProps[]>([
  {
    label: 'Fique por dentro',
    to:'',
    icon:'i-lucide-play'
  },
  {
    label:'Saiba mais.',
    to:'',
    color:'neutral',
    variant:'subtle',
    trailingIcon:'i-lucide-arrow-right'
  }  
])
</script>

<template>
  <UPageHero
    title="HomeTV"
    description="O lar dos melhores filmes você só encontra aqui! Acompanhe no nosso catálogo as informações do filme que você procura."
    headline="Seja bem-vindo!"
    orientation="horizontal"
    :links="links"
  />
</template>