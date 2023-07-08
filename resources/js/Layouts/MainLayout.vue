<template>
  
 <header class="border-b border-gray-200 dark:border-gray-700 bg-white dark:bg-gray-800 w-full">
    <div class="container mx-auto">
      <nav class="p-4 flex items-center justify-between">
        <div class="text-lg font-medium">
          <Link :href="route('listing.index')">Listings</Link>
        </div>
        <div class="text-xl text-indigo-600 dark:text-indigo-300 font-bold text-center">
          <Link :href="route('listing.index')">LaraZillow</Link>
        </div>
        <div>
          <Link :href="route('listing.create')" class="btn-primary">+ New Listing</Link>
        </div>
      </nav>
      <slot>Default</slot>
    </div>
  </header>
  

    <!-- <div v-if="flashSuccess" class="success">
      {{ flashSuccess }}
    </div> -->
  </template>
  
  <script setup>
  import { computed } from 'vue'
  import { Link, usePage } from '@inertiajs/vue3'
  

  
  const page = usePage()
  const flashSuccess = computed(
    () => page.props.value.flash.success,
  )
  </script>
  
