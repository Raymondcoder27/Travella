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
    <div id="ServiceSelectSmall">
        <div class="w-full rounded-2xl bg-custom-color h-[100px] relative">

            <div v-if="promo" class="">
                <div class="absolute top-1/3 left-1/3 transform -translate-x-1/4 -translate-y-1/4 mt-0.5">Promo</div>
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