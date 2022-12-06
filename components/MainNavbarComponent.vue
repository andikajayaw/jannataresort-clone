<template>
  <div id="mainNav" class="navbar-header">
    <div class="navbar-header-toggle">
      <div class="navbar-btn">
        <div class="navbar-btn-bars">
          <div></div>
          <div></div>
          <div></div>
        </div>
        <div class="navbar-btn-label">
          <span class="navbar-btn-label-menu">Menu</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.navbar-header {
  z-index: 5;
  position: fixed;
  right: -20px;
  background-color: #fff;
  cursor: pointer;
  z-index: 70;
  transition: all 0.7s cubic-bezier(0.19, 1, 0.22, 1);
  width: 80px;
  height: 110px;
  top: 30%;
  border: none;
  transform: translateX(0) translateY(-100%);
  color: #000;
}

.navbar-header .navbar-btn {
  position: absolute;
  width: 29px;
  height: 14px;
  margin: 0;
  transition: top 0.5s cubic-bezier(0.19, 1, 0.22, 1);
  top: auto;
  right: 35px;
  bottom: 75px;
  left: auto;
}

.navbar-header .navbar-btn-bars {
  position: absolute;
  right: 0;
  width: 65px;
  height: 15px;
  overflow: hidden;
}

.navbar-header .navbar-btn-label {
  position: absolute;
  top: 40px;
  right: 0;
  opacity: 1;
  transition: color 0.5s cubic-bezier(0.19, 1, 0.22, 1);
  font: 400 9px/1.3 Open Sans, sans-serif;
  letter-spacing: 2px;
  text-transform: uppercase;
  transition: all 0.7s cubic-bezier(0.19, 1, 0.22, 1);
  transform: translateX(7px) rotate(-90deg);
}

.navbar-header .navbar-btn-bars div:first-child {
  top: 7px;
}

.navbar-header .navbar-btn-bars div:nth-child(3) {
  top: 14px;
}

.navbar-header .navbar-btn-bars div {
  position: absolute;
  top: 0;
  right: 0;
  width: 25px;
  height: 1px;
  background-color: #000;
  transition: all 0.7s cubic-bezier(0.19, 1, 0.22, 1);
}

.navbar-header .navbar-btn-label {
  position: absolute;
  top: 40px;
  right: 0;
  opacity: 1;
  transition: color 0.5s cubic-bezier(0.19, 1, 0.22, 1);
  font: 400 9px/1.3 Open Sans, sans-serif;
  letter-spacing: 2px;
  text-transform: uppercase;
  transition: all 0.7s cubic-bezier(0.19, 1, 0.22, 1);
  transform: translateX(7px) rotate(-90deg);
}

.navbar-header .navbar-btn-label span {
  display: block;
  width: 40px;
}
</style>
