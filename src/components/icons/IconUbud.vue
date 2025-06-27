<script>
import imageSource from '@/assets/image/ubud.jpg'
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