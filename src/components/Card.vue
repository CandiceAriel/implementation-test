<template>
  <div class="card__wrapper">
    <div class="card__top">
      <div class='card-currency__wrapper'>
        <img src=".././assets/images/bitcoin_logo.svg" width="26" height="26">
        <span class='text_ext-bold'>{{ currency }}</span>-A88888
      </div>
      <div class='card-time__wrapper'>
        <span>Starts in <span class='text_ext-bold'>6d 10h 38m</span></span>
      </div>
    </div>
    <div class= 'card-detail__wrapper'>
      <div class='card-detail-annualized__container'>
        <span class='card-detail-annualized card-detail__title text_ext-bold'>Annualized<br><span class='card-detail__info text_ext-bold'>~100.00%</span></span>
      </div>
      <div class='card-detail-duration__container'>
        <span class='card-detail-duration card-detail__title text_ext-bold'>30Feb20 - 30Jul20<br><span class='card-detail__info text_ext-bold'>88 Days</span></span>
      </div>
      <div class='card-detail-cap card-detail-cap__container'>
        <p class='card-detail__title text_ext-bold'>Current / Cap</p>
        <p class='text_normal'>1,000,000 / 1,000,000 <span class='text_ext-bold'>BTC</span></p>
        <div></div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'CurrencyCard',
  props: {
    currency: String
  }
}
</script>