<script>
import imageSource from '@/assets/image/nusa.jpg'
export default {
    data() {
        return{
            imageSource: imageSource
        }
    }
}
</script>
<template>
   <img :src="imageSource" alt="" class="logo"/>
   </template>