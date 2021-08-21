<template>
  <main id="home">
    <!-- <img src="" alt=""> put svg of image here -->
    <h1 class="title">Garden Name</h1>
    <section class="garden">
      <plant-card v-for="item in 3" :key="item"></plant-card>
    </section>
  </main>
</template>

<script>
  import { defineAsyncComponent } from 'vue'

  export default {
    name: 'Home',
    components: {
      'plant-card': defineAsyncComponent(() => import('@/components/plant-card.vue'))
    }
  }
</script>

<style lang="scss" scoped>
  #home {
    display: flex; 
    flex-direction: column;
    justify-content: space-between;
    width: 100vw;
    height: 100%;
    .title {
      left: 10px;
    }
  }
  .garden {
    margin-top: 20px;
  }
</style>
