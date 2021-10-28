<template>
  <footer class="footer mt-5">
    <div class="footer__content">
      <div class="footer__company">
        <span>© Kolesa Group</span>
        <div class="sns-icons">
          <a href="#"><img src="@/assets/instagram.svg" width="18" height="18" alt=""></a>
          <a href="#" ><img src="@/assets/youtube.svg" width="18" height="18" alt=""></a>
          <a href="#"><img src="@/assets/vk.svg" width="18" height="18" alt=""></a>
        </div>
      </div>
      <div class="contact-company">
        <div class="mr">
          <span>Есть идеи что улучшить?<br> Не знаешь, с кем решить проблему?</span>
        </div>
        <button class="contact-company__button">Написать</button>
      </div>
    </div>
  </footer>
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

@mixin flexCenter {
  display: flex;
  justify-content: center;
  align-self: center;
}

.footer {
  background-color: $black-primary-color;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.12);
  box-sizing: border-box;
  width: 100%;
  text-align: left;
  padding: 16px 8px;
  bottom: 0;

  &__content {
    display: flex;
    justify-content: space-between;
  }

  &__company {
    color: $primary-color;
    font-weight: $font-regular;
    font-size: $small-font-size;
    line-height: 24px;
  }
}

.contact-company {
  @include flexCenter;

  color: $primary-color;
  font-size: $small-font-size;
  font-weight: $font-regular;

  &__button {
    box-shadow: 0 2px 4px rgba(28, 24, 25, 0.1);
    border-radius: 8px;
    border: 0;
    color: $blue-primary-color;

    @include flexCenter;

    padding: 12px 50px;
    cursor: pointer;
  }
  .sns-icons {
    @include flexCenter;
  }

}
.mt-5 {
  margin-top: 8em;
}

.mr {
  margin-right: 16px;
}
.ml-1 {
  margin-left: 10px;
}
</style>
