<template>
  <div class="mt">
    <div class="flex-row">
      <div class="card ml mb">
        <div class="image">
          <img width="330" height="330" src="@/assets/t-shirt.png" alt="product-img">
          <span class="image__badge">new</span>
        </div>
        <div class="description">
          <div class="description__price">
            220 баллов
          </div>
          <h3 class="description__title">
            Футболка "Эволюционируй или ...
          </h3>
          <div class="description__hint">
            Размеры S/M/L
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

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

.mt {
  margin-top: 16px;
}
.flex-row {
  display: flex;
  flex-flow: wrap;
}
.image {
  position: relative;

  &__badge {
    position: absolute;
    bottom: 16px;
    left: 16px;
    font-size: $extra-small-font-size;
    line-height: 20px;
    background: $green-color;
    color: $primary-color;
    padding: 0 4px;
    border-radius: 4px;
    text-transform: uppercase;
  }
}
.card {
  box-shadow: 0 2px 10px rgba(28, 24, 25, 0.1);
  border-radius: 8px;
  width: 330px;
}

.description {
  padding: 16px;

  &__price {
    font-weight: $font-semi-bold;
    font-size: $extra-large-font-size;
    line-height: 36px;
    color: $blue-primary-color;
    margin-bottom: 8px;
  }

  &__title {
    margin-bottom: 4px;
    font-size: $medium-font-size;
    line-height: 24px;
    font-weight: $font-semi-bold;
  }

  &__hint {
    color: $gray-color;
    font-size: $small-font-size;
    line-height: 24px;
  }
}
.mb {
  margin-bottom: 14px;
}
.ml {
  margin-left: 14px;
}
</style>
