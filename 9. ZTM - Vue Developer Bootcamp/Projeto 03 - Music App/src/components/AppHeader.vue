<template>

  <header id="header" class="bg-gray-700">
    <nav class="container mx-auto flex justify-start items-center py-5 px-4">
      <!-- App Name -->
      <a class="text-white font-bold uppercase text-2xl mr-4" href="#"
        >Music</a
      >

      <div class="flex flex-grow items-center">
        <!-- Primary Navigation -->
        <ul class="flex flex-row mt-1">
          <!-- Navigation Links -->
          <li>
            <a class="px-2 text-white" href="#" @click.prevent="modalStore.isOpen = !modalStore.isOpen">Login / Register</a>
          </li>
          <li>
            <a class="px-2 text-white" href="#">Manage + {{ modalStore.hiddenClass }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>

</template>

<script setup>
// PINIA STORES
import { useModalStore } from '@/stores/modalStore'
const modalStore = useModalStore()
</script>
