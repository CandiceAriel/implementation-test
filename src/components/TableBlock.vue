<template>
  <div class="annualized__wrapper">
    <div class="dropdown dropdown--small">
      <span>All</span>
      <img class="icon__triangle-down--dropdown" src=".././assets/images/triangle-down-black.svg">
    </div>
    <table class="annualized annualized__table">
      <thead>
        <tr class="annualized annualized__table-head">
          <th class="text--algn-left">Block</th>
          <th class="text--algn-right"><span>Annualized</span> <img class="icon__triangle-down" src=".././assets/images/triangle-down.svg"></th>
          <th class="text--algn-right"><span>Date</span> <img class="icon__triangle-down" src=".././assets/images/triangle-down.svg"></th>
          <th class="text--algn-right"><span>Duration</span> <img class="icon__triangle-down" src=".././assets/images/triangle-down.svg"></th>
          <th class="text--algn-left"><span>Current/Cap</span></th>
          <th class="text--algn-left"><span></span></th>
          <th><span>Status</span></th>
          <th></th>
        </tr>
      </thead>
      <tbody>
        <tr
          class="annualized annualized__table-row"
          v-for="(item, index) in annualized"
          :key="index"
        >
          <td class="text--algn-left">
            <img class="annualized__coin-symbol" src=".././assets/images/Bitcoin-BTC-icon.svg">
            <span class="text--ext-bold">{{ item.blockCurrency }}</span> -
            {{ item.blockCode }}
          </td>
          <td class="text--algn-right">
            <span class="text--ext-bold">{{ item.annualized }}</span>
           
          </td>
          <td class="text--algn-right">
            <span>{{ item.date }}</span>
          </td>
          <td class="text--algn-right">
            <span>{{ item.duration }}</span>
          </td>
          <td class="text--algn-left">
            <span
              >{{ item.currentCap }}
              <span class="text--ext-bold">{{
                item.currentCapCurrency
              }}</span></span
            >
            <div
              class="progress-bar__wrapper progress-bar__wrapper--gray progress-bar__moved"
            >
              <div class="progress-bar__bar progress-bar__bar--small"></div>
              <div class="loader" style="--n: 1; --f: 0"></div>
            </div>
          </td>
          <td class="text--algn-left">
            <span>{{ item.cap }}</span>
            <div
              class="progress-bar__wrapper progress-bar__wrapper--gray progress-bar__moved"
            >
              <div class="progress-bar__bar progress-bar__bar--small"></div>
              <div class="loader" style="--n: 1; --f: 0"></div>
            </div>
          </td>
          <td>
            <div class="status__time status__time--secondary">
              <span
                >Starts in
                <span class="text--ext-bold"
                  >{{ item.startTimeDays }}d {{ item.startTimeHours }}h
                  {{ item.startTimeMins }}m</span
                ></span
              >
            </div>
          </td>
          <td>
            <button class="btn btn__submit btn__submit--small">
              <span>Subscribe</span>
            </button>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "TableBlock",
  data() {
    return {
      annualized: [
        {
          blockCurrency: "PAX",
          blockCode: "A88888",
          annualized: "~100.00%",
          date: "30Feb20 - 30Jul20",
          duration: "88 days",
          currentCap: "1,000,000 / 1,000,00",
          currentCapCurrency: "BTC",
          cap: "1",
          startTimeDays: " 88",
          startTimeHours: "88",
          startTimeMins: "88",
        },
        {
          blockCurrency: "PAX",
          blockCode: "A88888",
          annualized: "~100.00%",
          date: "30Feb20 - 30Jul20",
          duration: "88 days",
          currentCap: "1,000,000 / 1,000,00",
          currentCapCurrency: "BTC",
          cap: "1",
          startTimeDays: " 88",
          startTimeHours: "88",
          startTimeMins: "88",
        },
        {
          blockCurrency: "PAX",
          blockCode: "A88888",
          annualized: "~100.00%",
          date: "30Feb20 - 30Jul20",
          duration: "88 days",
          currentCap: "1,000,000 / 1,000,00",
          currentCapCurrency: "BTC",
          cap: "1",
          startTimeDays: " 88",
          startTimeHours: "88",
          startTimeMins: "88",
        },
        {
          blockCurrency: "PAX",
          blockCode: "A88888",
          annualized: "~100.00%",
          date: "30Feb20 - 30Jul20",
          duration: "88 days",
          currentCap: "1,000,000 / 1,000,00",
          currentCapCurrency: "BTC",
          cap: "1",
          startTimeDays: " 88",
          startTimeHours: "88",
          startTimeMins: "88",
        },
        {
          blockCurrency: "PAX",
          blockCode: "A88888",
          annualized: "~100.00%",
          date: "30Feb20 - 30Jul20",
          duration: "88 days",
          currentCap: "1,000,000 / 1,000,00",
          currentCapCurrency: "BTC",
          cap: "1",
          startTimeDays: " 88",
          startTimeHours: "88",
          startTimeMins: "88",
        },
      ],
    };
  },
};
</script>

<style>
</style>