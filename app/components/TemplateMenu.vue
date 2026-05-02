<template>
  <UHeader>
    <template #left>
      <div class="flex items-center gap-2">
       <NuxtLink to="/">
         <img
        src="/iconehometv.png"
        type="select"
        alt='ìcone HomeTV'
        class="h-10 w-auto grid grid-cols-1 rounded-lg shadow-2xl ring ring-default"
        to='/index.vue'
        >
       </NuxtLink>
        <h1 class="font-bold text-xl">HomeTV</h1>
      </div>
    </template>
     <template #right>
      <div class="flex items-center gap-2">
        <UButton
        to='/Login'
        icon="i-lucide-circle-user" 
        label="Login"
        variant="solid"
        color="primary"
          />
      </div>
    </template>
    </UHeader>
</template>
    