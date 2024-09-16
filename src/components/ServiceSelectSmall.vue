<script setup>
    import {toRefs, defineProps} from 'vue'

    const props = defineProps({
        text: String,
        image: String
    })

    const { text, image} = toRefs(props)
</script>

<template>
    <div id="ServiceSelectSmall">
        <div class="w-full rounded-2xl bg-custom-color h-[100px] relative">

            <div v-if="promo" class="">
                <div class="absolute top-1/3 left-1/3 transform -translate-x-1/4 -translate-y-1/4 mt-0.5">Promo</div>
                <img :width="imageWidth" :src="'/public/uber/'+image+'.png'" alt="">

            </div>
            <div class="flex justify-between p-2">
                <div class="text-xs text-center text-gary-900 mt-2">
                    {{text}}
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