<script setup>
defineProps({
  nama: {
    type: String,
    required: true,
  },
  harga: {
    type: String,
    required: true,
  },
})


</script>
<template>
  <div class='box'>
    <slot name='images'></slot>
    <!-- <div class='img-box'>
    </div> -->
    <div class= 'bottom'>
      <p>{{ nama }}</p>
      <h1>harga mulai dari
      </h1>
      <p><strong>Rp.{{ harga }}</strong></p>
    </div>
    <button>
      <slot></slot></button>
    </div>
   

</template>

<style scoped>
</style>
