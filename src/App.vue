<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>

  <header>
    <img alt="logo" class="logohead" src="./assets/logo aksara bali-02.png" width="270" height="200" />
    <div class="judul">HalloBali</div>
 </header>
  <div class="data">
    <div class="wrapper">
      <HelloWorld msg="Travelers Favorites: Bali's Best Picks" />
    </div>
  <TheWelcome />
</div>

</template>

<style scoped>

header {
  font-size: 3rem;
  color: white;
  padding: 0.2rem;
  display: flex;
  border-bottom: 1px solid #e30f0f;
  border-bottom-right-radius: 5px;
  border-bottom-left-radius: 5px;
  top: 0;
  flex-direction: row;
  left: 0;
  right: 0;
  bottom: 10;
  justify-content: baseline;
  background-color: #a22840;
}

.logohead {
  display: block;
  margin: 0;
  max-width: 100%;
  width: 180px;
  height: 100px;
}
header .judul{
  font-size: 3rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;

  }
  .logohead {
    margin: 0 2rem 0 0;
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
