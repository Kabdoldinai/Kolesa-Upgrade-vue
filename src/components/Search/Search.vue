<template>
  <div class="box">
    <div class="space-between">
      <div class="search search--mt">
        <input type="text" name="search" placeholder="Поиск">
      </div>
      <div class="user">
        <a href="#"><img class="user__profile"
                         src="@/assets/user-profile.png" alt="user-avatar">
        </a>
        <div class="user__info">
          <a href="#" class="user__name bold">Мортиджан</a>
          <a href="#">300 баллов</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
$medium-large-font-size: 18px;

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

.search {
  font-size: $medium-large-font-size;

  input {
    -webkit-appearance: textfield;
    -webkit-box-sizing: content-box;
    padding: 12px 16px 9px 36px;
    min-width: 300px;
    background: #f2f2f3 url('../../assets/search-icon.svg') no-repeat 9px center;
    -webkit-border-radius: 10em;
    -moz-border-radius: 10em;
    border-radius: 8px;
    -webkit-transition: all 0.5s;
    -moz-transition: all 0.5s;
    transition: all 0.5s;
    border: none;

    &:focus {
      outline: none;
    }
  }

  &--mt {
    margin-top: 22px;
  }
}

.user {
  font-size: $extra-small-font-size;
  font-weight: $font-regular;
  display: flex;

  &__info {
    margin-left: 12px;
    display: flex;
    flex-direction: column;
  }

  &__profile {
    border-radius: 50%;
  }

  &__name {
    line-height: 24px;
    color: $blue-primary-color;
  }
}

.box {
  width: 100%;
}
.space-between {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}

</style>
