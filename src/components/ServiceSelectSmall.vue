<script setup>
import { toRefs, defineProps } from "vue";

const props = defineProps({
  text: String,
  image: String,
});

const { text, image } = toRefs(props);
</script>

<template>
  <div id="ServiceSelectSmall">
    <div class="w-full rounded-2xl bg-custom-color h-[100px] relative">
        <div
          class="absolute top-1/3 left-1/3 transform -translate-x-1/4 -translate-y-1/4 mt-0.5"
        >
        <img width="55" :src="'/public/uber/' + image + '.png'" alt="" />
        </div>
    </div>
    <div class="text-xs text-center text-gary-900 mt-2">
      {{ text }}
    </div>
  </div>
</template>

<style scoped>
.bg-custom-color {
  background-color: rgb(237, 237, 237);
}
</style>