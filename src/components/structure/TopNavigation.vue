<template>
  <nav class="w-full px-4 bg-black relative z-20 text-white-200">
    <div class="container mx-auto max-w-4xl h-16 flex justify-between text-xs md:text-sm">
      <div class="h-full flex items-center">
        <router-link to="/" class="flex justify-center items-center">
          <div class="text-white text-2xl">{{firstName}}</div>
        </router-link>
      </div>
      <div class="h-full flex items-center">
        <FullScreenModal/>
      </div>
    </div>
  </nav>
</template>

<script setup>
import FullScreenModal from './FullScreenModal.vue'
import { storeToRefs } from 'pinia'
import {useUserStore} from '../../store/user-store'

// access the `store` variable anywhere in the component ✨
const userStore = useUserStore()
const { firstName } = storeToRefs(userStore)

</script>