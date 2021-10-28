<template>
  <div class="menu">
    <img src="@/assets/main-logo.svg" alt="company-logo">
    <ul class="menu menu__list">
      <li class="menu--mt"><a href="#">Оргсхема</a></li>
      <li class="menu--mt"><a href="#">Kolesa <span class="bold">Team</span></a></li>
      <li class="menu--mt"><a href="#">Картина компании</a></li>
      <li class="menu--mt"><a href="#">Новости</a></li>
      <li class="menu--mt"><a href="#">Education</a></li>
      <li class="menu--mt"><a href="#">Guidelines</a></li>
      <li class="menu--mt"><a href="#">Библиотека</a></li>
      <li class="menu--mt"><a href="#">FAQ</a></li>
    </ul>
  </div>
</template>

<script>

export default {
  name: 'SideMenu',
};
</script>

<style lang="scss">
$blue-primary-color: #2a81dd;
$medium-font-size: 16px;

.menu {
  list-style: none;
  text-decoration: none;
  position: relative;
  font-size: $medium-font-size;
  padding: 24px;

  &__list {
    padding: 0;
  }

  &--selected {
    background: $blue-primary-color;
    border-radius: 10px;
    transform: matrix(-1, 0, 0, 1, 0, 0);
    width: 4px;
    height: 36px;
    position: absolute;
    margin: -8px -8px;
  }

  &--mt {
    margin-top: 22px;
  }
}

</style>
