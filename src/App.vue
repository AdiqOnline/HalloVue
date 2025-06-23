<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
<div class="data">
  <header>
    <img alt="logo" class="logo" src="./assets/image/gapura-backtobali.png" width="260" height="200" />
  <div class="wrapper">
      <HelloWorld msg="HalloBali!" />
    </div>
  </header>
<main>
  <TheWelcome />
</main>
</div>

</template>

<style scoped>
.data {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;

  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
