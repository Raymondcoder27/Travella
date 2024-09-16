<script setup>
// import TheWelcome from '../components/TheWelcome.vue'
import ServiceSelectLarge from '@/components/ServiceSelectLarge.vue';
</script>

<template>
  <main id="Home" class="flex flex-col h-screen">
    <div class="m-3 mb-auto">
      <div class="grid grid-cols-2 gap-3 my-3">
        <ServiceSelectLarge 
        text="Ride"
        imageWidth="74"
        image="ride"/>
      <ServiceSelectLarge 
        text="Food"
        imageWidth="74"
        image="ride"/>
      </div>
    </div>
    <!-- <TheWelcome /> -->
  </main>
</template>
