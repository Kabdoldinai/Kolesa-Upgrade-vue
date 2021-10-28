<template>
  <div class="score mt">
    <button class="score-button score-button--green" type="button">
      <img src="@/assets/plus-icon.svg" width="30" alt="plus-icon">
      <span class="ml">Получить баллы</span>
    </button>
    <button class="score-button score-button--yellow ml" type="button">
      <img src="@/assets/question-icon.svg" width="30" alt="question-icon">
      <span class="ml">Как получить баллы</span>
    </button>
    <button class="score-button score-button--blue ml" type="button">
      <img src="@/assets/gift-icon.svg" width="30" alt="gift-icon">
      <span class="ml">Подарить баллы</span>
    </button>
  </div>
</template>

<style lang="scss">
$large-font-size: 20px;
$font-semi-bold: 600;
$payed-green-color: #eff8eb;
$payed-blue-color: #e9f2fb;
$payed-yellow-color: #fffae7;

.score-button {
  border: none;
  border-radius: 16px;
  background: transparent;
  min-width: 350px;
  padding: 12px;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  font-size: $large-font-size;
  font-weight: $font-semi-bold;
  flex-flow: wrap;

  &--green {
    background: $payed-green-color;
  }

  &--yellow {
    background: $payed-yellow-color;
  }

  &--blue {
    background: $payed-blue-color;
  }

  &:hover {
    box-shadow: 0 4px 6px 0(0, 0, 0, 0.4);
    background-color: #d1d2e6;
  }
}
.mt {
  margin-top: 16px;
}

.ml {
  margin-left: 14px;
}

</style>
