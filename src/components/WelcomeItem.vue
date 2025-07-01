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
      <br/>
      <h1>*harga mulai dari</h1>
      <p><strong>Rp.{{ harga }}</strong></p>
    </div>
    <button v-on:click="klik">
      <slot></slot></button>
    </div>
</template>

<style scoped>
  .bottom{
    margin-top: 20px;
    width: 100%;
    /* text-align: center; */
    display: flex;
    flex-direction: column;
    /*align-items: center;*/
    justify-content: space-between;
    padding-top: 20px auto;
    align-items: left;
    font-size: 20px;
  }
.bottom h1 {
  font-style: italic;
  /*position: relative;*/
  font-size: 16px;
  color: grey;
}
p {
  font-size: 1rem;
}
p strong{
  font-size: 1.8rem;
  color: black;
}
.box{
  display:flex;
  flex-direction: column;
  /*align-items: center;*/
  justify-content: space-between;
  border: 1px solid grey;
  border-radius: 5px;
  padding-bottom:10px;
  /*justify-content: center;*/
  }
.icon{
  display: flex;
  align-items: center;
  flex-direction: column;
}
</style>
