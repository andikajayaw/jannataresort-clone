<template>
  <div id="navMobile" class="navbar-header-mobile" data-v-4a9d7f1f="">
    <a class="logo" data-v-4a9d7f1f=""
      ><img src="/_nuxt/img/1336c61.png" alt="" data-v-4a9d7f1f=""
    /></a>
    <div id="navMobileBtn" class="navbar-btn-bars" data-v-4a9d7f1f="">
      <div data-v-4a9d7f1f=""></div>
      <div data-v-4a9d7f1f=""></div>
      <div data-v-4a9d7f1f=""></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@media screen and (max-width: 540px) {
  .navbar-header-mobile {
    display: block;
  }
}

.navbar-header-mobile {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 80px;
  background-color: #323037;
  z-index: 999;
}

.navbar-header-mobile .logo {
  width: 70px;
  display: block;
  margin: 10px auto;
}

.navbar-header-mobile .navbar-btn-bars {
  position: absolute;
  right: 30px;
  top: 30px;
  width: 65px;
  height: 15px;
  overflow: hidden;
}

.navbar-header-mobile .navbar-btn-bars div:first-child {
  top: 7px;
}

.navbar-header-mobile .navbar-btn-bars div:nth-child(3) {
  top: 14px;
}

.navbar-header-mobile .navbar-btn-bars div {
  position: absolute;
  top: 0;
  right: 0;
  width: 25px;
  height: 1px;
  background-color: #fff;
  transition: all 0.7s cubic-bezier(0.19, 1, 0.22, 1);
}
</style>
