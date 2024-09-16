<script setup>
// import TheWelcome from '../components/TheWelcome.vue'
import ServiceSelectLarge from '@/components/ServiceSelectLarge.vue';
import ServiceSelectSmall from '@/components/ServiceSelectSmall.vue';
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
      <div class="grid grid-cols-4 gap-3 my-3">
        <ServiceSelectSmall 
        text="Ride"
        image="ride"/>
      <!-- <ServiceSelectSmall 
        text="Food"
        imageWidth="74"
        image="food"
        :promo="true"/> -->
      </div>
    </div>
    <!-- <TheWelcome /> -->
  </main>
</template>
