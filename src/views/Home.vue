<template>
  <div class="home__wrapper">
    <CardComponent msg="Welcome to Your Vue.js App"/>
    <CardComponent msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import CardComponent from '../components/Card.vue';

export default {
  name: 'ViewHome',
  components: {
    CardComponent
  }
}
</script>

<style>

</style>