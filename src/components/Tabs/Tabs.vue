<template>
  <div class="tabs mt-2">
    <button class="tab-button score-button--blue">Все товары</button>
    <button @click="isShowClothes = !isShowClothes"
            class="tab-button tab-button__transparent ml-1">Одежда</button>
    <button
            @click="isShowAccessories = !isShowAccessories"
            class="tab-button tab-button__transparent ml-1">Аксессуары</button>
  </div>
</template>

<script>

import axios from 'axios';

export default {
  name: 'Tabs',
  props: {
    clothesShow: Array,
    accessoriesShow: Array,
  },
  data() {
    return {
      clothes: [],
      accessories: [],
      isShowAllProducts: false,
      isShowClothes: false,
      isShowAccessories: false,
    };
  },
  mounted() {
    const config = { headers: { Authorization: `Bearer ${'rhhrmjvdvcv0ka4e6ouao9a1gj42fbjim5bcu60f'}` } };
    axios.get(
      'https://api.json-generator.com/templates/-_RLsEGjof6i/data',
      config,
    ).then((res) => {
      this.clothes = res.data;
    });
    axios.get(
      'https://api.json-generator.com/templates/q3OPxRyEcPvP/data',
      config,
    ).then((res) => {
      this.accessories = res.data;
    });
  },
  methods: {
    showClothes() {
      this.isShowClothes = true;
    },
  },
};

</script>

<style lang="scss">

$primary-color: #fff;
$black-primary-color: #1c1819;
$blue-primary-color: #2a81dd;
$blue-lighter: #d6ecfb;
$red-color: #f33;
$gray-color: #888b94;
$green-color: #64bd38;
$payed-blue-color: #e9f2fb;
$payed-yellow-color: #fffae7;
$payed-green-color: #eff8eb;
$font-regular: 400;
$font-semi-bold: 600;
$extra-small-font-size: 13px;
$small-font-size: 14px;
$medium-font-size: 16px;
$medium-large-font-size: 18px;
$large-font-size: 20px;
$extra-large-font-size: 24px;

.tab-button {
  border: none;
  border-radius: 8px;
  min-width: 120px;
  padding: 12px;
  cursor: pointer;

  &__transparent {
    border: 1px solid rgb(223, 222, 222);
    box-sizing: border-box;
    border-radius: 8px;
    background: $primary-color;
    color: $blue-primary-color;
    font-weight: $font-regular;
    font-size: $small-font-size;
  }

  &:hover {
    background: $payed-blue-color;
    border: none;
  }
}
.mt-2 {
  margin-top: 24px;
}

.ml-1 {
  margin-left: 6px;
}

</style>
