<script setup>
    import {toRefs, defineProps} from 'vue'

    const props = defineProps({
        text: String,
        imageWidth: String,
        image: String
    })

    const { text, imageWidth, image} = toRefs(props)
</script>

<template>
    <div id="ServiceSelectLarge">
        <div class="w-full rounded-2xl bg-custom-color h-[100px]">

            <div class="w-full relative z-10">
                <span class="absolute bg-green-700 text-gray-100 text-xs rounded-3xl top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 p-0.5 px-2">Promo</span>
            </div>
            <div class="flex justify-between p-2">
                <div class="text-lg ml-2 text-gary-900 mt-14">
                    {{text}}
                </div>
                <div class="mt-3 mr-1">
                    <img :width="imageWidth" :src="'/public/uber/'+image+'.png'" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .bg-custom-color{
        background-color:rgb(237,237,237)
    }
</style>