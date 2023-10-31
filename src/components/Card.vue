<template>
  <div class="card__wrapper" :class="{'card__wrapper-right': isRight}">
    <div class="card card__header">
      <div class='card__header-currency'>
        <img src=".././assets/images/bitcoin_logo.svg" width="26" height="26">
        <span class='text--ext-bold'>{{ currency }}</span>-A88888
      </div>
      <div class='status__time status__time--primary'>
        <span>Starts in <span class='text--ext-bold'>{{startTimeDays}}d {{startTimeHours}}h {{startTimeMinutes}}m</span></span>
      </div>
    </div>
    <div class= 'card card__content'>
      <div class='card__annualized'>
        <span class='content__title text--ext-bold'>Annualized<br><span class='content__info text--ext-bold'>~100.00%</span></span>
      </div>
      <div class='card__duration'>
        <span class='content__title text--ext-bold'>30Feb20 - 30Jul20<br><span class='content__info text--ext-bold'>88 Days</span></span>
      </div>
      <div class='card__cap'>
        <p class='content__title text--ext-bold'>Current / Cap</p>
        <p class='text_normal'>1,000,000 / 1,000,000 <span class='text--ext-bold'>{{ currency }}</span></p>
        <div class="progress-bar__wrapper progress-bar__moved">
          <div class="progress-bar__bar"></div>
          <div class="loader" style="--n: 1; --f: 0;"></div>
        </div>
      </div>
      <button class='btn btn__submit btn__submit--big'>
        <span>Subscribe</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CurrencyCard',
  props: {
    currency: String,
    startTimeDays: String,
    startTimeHours: String,
    startTimeMinutes: String,
    isRight: Boolean
  },
  data(){
    return {
    }
  }
}
</script>