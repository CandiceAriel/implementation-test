<template>
  <div class="home__wrapper">
    <CurrencyCard currency="BTC"/>
    <CurrencyCard currency="ETH"/>
  </div>
</template>

<script>
import CurrencyCard from '../components/Card.vue';

export default {
  name: 'ViewHome',
  components: {
    CurrencyCard
  }
}
</script>

<style>

</style>