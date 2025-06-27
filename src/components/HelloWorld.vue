<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
  
})
</script>

<template>
  <div class="top">
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Welcome to Bali, where unforgettable experiences await. In this curated selection, discover Bali's best picks - the absolute must-see attractions, activities, and tours that have captivated travelers before you. Immerse yourself in breathtaking natural wonders, embrace rich cultural encounters, embark on thrilling adventures, and find serene escapes. These are the handpicked gems that epitomize the magic of Bali. Join us on this journey as we unveil the essence of Bali's tourism offerings. Get ready to create lasting memories in this enchanting paradise. Enjoy the best of Bali all in one place.
      </h3>
  </div>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
}
h3 {
  font-size: 1.1rem ;
  color: rgb(0, 0, 0);
}
.greetings h1,
.greetings h3 {
  text-align: center;
}
@media (min-width: 500px) {
  .greetings h1,
  .greetings h3 {
    text-align: justify;
  }
}
</style>
