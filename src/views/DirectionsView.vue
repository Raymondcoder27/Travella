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
          <div :class="[isPickUpActive ? 'circle-black' : 'circle-gray']"></div>
             <div class="line"></div>
          <div :class="[!isPickUpActive ? 'square-black' : 'square-gray']"></div>
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
  .circle-black{
    margin: 0 auto;
    width: 9px;
    height: 9px;
    background-color: black;
    border-radius: 100%;
  }

  .circle-gray{
    margin: 0 auto;
    width: 9px;
    height: 9px;
    background-color: rgb(191, 191, 191);
    border-radius: 100%;
  }

  .square-black{
    margin: 0 auto;
    width: 9px;
    height: 9px;
    background-color: black;
  }

  .square-gray{
    margin: 0 auto;
    width: 9px;
    height: 9px;
    background-color: rgb(191, 191, 191);
  }

  .line{
    margin: 0 auto;
    width: 2px;
    height: 9px;
    background-color: rgb(191, 191, 191);
  }
/* } */
</style>