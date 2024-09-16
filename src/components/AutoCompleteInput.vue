<script>
    import {toRefs, defineProps, defineEmits} from 'vue'

    const emit = defineEmits(['update:input', 'clearInput', 'isActive'])

    const props = defineProps({
        theId:String,
        imageWidth: String,
        image:String,
        promo: {Boolean, default:false}
    })
    const {text,imageWidth, image} = toRefs(props)
</script>

<template>
    <div id="AutoCompleteInput" class="flex items-center">
        <input
        :id="theId" v-model="inputComputed"
        @click="emit('isActive', true)" 
        type="text" 
        class="text-md bg-gray-100 appearance-none w-full py-2.5 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline focus:bg-gray-200"
        placeholder="placeholder"
        autocomplete="off">
    </div>
</template>

<style scoped>

</style>