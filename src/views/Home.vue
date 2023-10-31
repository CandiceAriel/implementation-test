<template>
  <div class="home__wrapper">
    <CurrencyCard currency="BTC" startTimeDays="6" startTimeHours="10" startTimeMinutes="38" :isRight="false"/>
    <CurrencyCard currency="ETH" startTimeDays="6" startTimeHours="10" startTimeMinutes="38" :isRight="true"/>
    <TableBlock />
  </div>
</template>

<script>
import CurrencyCard from '../components/Card.vue';
import TableBlock from '../components/TableBlock.vue'

export default {
  name: 'ViewHome',
  components: {
    CurrencyCard,
    TableBlock
  }
}
</script>

<style>

</style>