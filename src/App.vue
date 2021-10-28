<template>
  <div id="app">
    <section class="container">
    <SideMenu />
      <div class="content">
        <div class="space-between">
          <Search />
        </div>
        <Banner />
        <ScoreButtons/>
        <Tabs />
        <Products />
      </div>
    </section>
    <Footer />
  </div>
</template>

<script>
import SideMenu from './components/SideMenu/SideMenu.vue';
import Search from './components/Search/Search.vue';
import Banner from './components/Advertise/Advertise.vue';
import ScoreButtons from './components/ScoreButtons/ScoreButtons.vue';
import Tabs from './components/Tabs/Tabs.vue';
import Products from './components/Products/Products.vue';
import Footer from './components/Footer/Footer.vue';

export default {
  name: 'App',
  components: {
    Search,
    SideMenu,
    Banner,
    ScoreButtons,
    Tabs,
    Products,
    Footer,
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap');

#app {
  font-family: 'Open Sans', sans-serif;
  margin: 0;
  padding: 0;
}
a,
a:hover,
a:focus,
a:active {
  text-decoration: none;
  color: inherit;
}

.container {
  box-sizing: border-box;
  display: flex;
  padding: 8px;
}

.content {
  width: 78%;
}

.space-between {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}

</style>
