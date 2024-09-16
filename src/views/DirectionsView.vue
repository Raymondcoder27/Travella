<script setup>
  import ArrowIcon from 'vue-material-design-icons/ArrowLeft.vue'
</script>

<template>
  <main id="Directions" class="flex flex-col h-screen">
    <div class="grid grid-cols-12 mt-4 shadow-md">
      <div class="col-span-2 mx-auto">
        <div>
          <ArrowIcon :size="35"/>
        </div>

        <div class="h-16 mt-4 w-full">
          <div></div>
        </div>
      </div>
    </div>
  </main>
</template>
<style scoped>
/* #ServiceSelectSmall{ */
    .bg-custom-color {
        background-color: rgb(237, 237, 237);
}
/* } */
</style>