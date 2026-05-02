<script setup lang="ts">
import type { AuthFormField } from '@nuxt/ui'

const fields = ref<AuthFormField[]>([
  {
    name: 'E-mail',
    type: 'email',
    label: 'Email',
    placeholder: 'Digite seu e-mail',
    required: true
  },
  {
    name: 'Senha',
    type: 'password',
    label: 'Password',
    placeholder: 'Digite sua senha',
    required: true
  },
  {
    name: 'País de Origem',
    type: 'select',
    label: 'Country',
    placeholder: 'País de Origem',
    items: [
      {
        label: 'Estados Unidos',
        value: 'us'
      },
      {
        label: 'França',
        value: 'fr'
      },
      {
        label: 'Reino Unido',
        value: 'uk'
      },
      {
        label: 'Austrália',
        value: 'au'
      }
    ]
  },
  {
    name: 'remember',
    type: 'checkbox',
    label: 'Remember me',
    description: 'You will be logged in for 30 days.'
  }
])
</script>

<template>
<div>
  <UAuthForm :fields="fields" class="max-w-sm" />
  </div>
</template>