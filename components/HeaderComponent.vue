<template>
  <header id="header" class="header">
    <div class="q-container">
      <div class="columns">
        <div class="column logo-wrap">
          <a href="/en" class="logo"
            ><img src="~/assets/images/jannata-logo.png" alt=""
          /></a>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.columns {
  display: flex;
}

#header.logo-wrap {
  position: absolute;
  left: 50%;
  top: 80px;
  transform: translateX(-50%);
  z-index: 10;
}

.column {
  display: block;
  flex-basis: 0;
  flex-grow: 1;
  flex-shrink: 1;
}

#header.logo-wrap.logo {
  display: inline-block;
  max-width: 120px;
}

img {
  max-width: 100%;
  vertical-align: middle;
  border-style: none;
}
</style>
