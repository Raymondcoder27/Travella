<script setup>
// import TheWelcome from '../components/TheWelcome.vue'
import ServiceSelectLarge from '@/components/ServiceSelectLarge.vue';
import ServiceSelectSmall from '@/components/ServiceSelectSmall.vue';
import MagnifyIcon from 'vue-material-design-icons/Magnify.vue'
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
        image="food"
        :promo="true"/>
      </div>
      <div class="grid grid-cols-4 gap-3 my-4">
        <ServiceSelectSmall 
        text="2 Wheels"
        image="2wheels"/>
        <ServiceSelectSmall 
        text="Transit"
        image="transit"/>
        <ServiceSelectSmall 
        text="Reserve"
        image="reserve"/>
        <ServiceSelectSmall 
        text="Travel"
        image="travel"/>
      </div>

      <div class="w-full bg-custom-color h-14 rounded-full flex items-center p-3">
        <MagnifyIcon size="40"/>
        <div class="ml-3 text-xs font-semibold">
          Enter pickup location
        </div>
      </div>
    </div>
  </main>
</template>
