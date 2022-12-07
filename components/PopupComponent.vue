<template>
  <div class="popup popup-homepage open">
    <div class="popup-container">
      <div class="block-content-wrap">
        <div class="columns">
          <div class="close">
            <i class="icon icon-plus"></i>
          </div>
          <figure class="column picture">
            <div class="wrap">
              <img
                src="https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com/5e65fe109dae8c14dd70f7e0/pictures/homepage/15882279350951/big/DJI_0587_JPG.jpg"
                alt=""
              />
            </div>
          </figure>
          <div class="column entry">
            <div class="inner">
              <span class="section-headline lines-middle text-gold"
                >Plan Your Ubud Escape</span
              >
              <span class="title">STAY SAFE</span>
              <div class="desc">
                <p>
                  Reserve your Bali holiday with no quarantine as we are a
                  certified CHSE resort in the heart of Ubud.&nbsp;
                </p>
              </div>
              <a
                href="https://chse.kemenparekraf.go.id/detail-tersertifikasi/perhotelan-101"
                class="button"
                ><i class="icon icon-angle-right"></i>
                View Certificate Here
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.popup-homepage.open {
  opacity: 1;
  visibility: visible;
  transform: translateZ(0);
}
.popup-homepage {
  position: absolute;
  top: calc(100vh - 230px);
  right: 25px;
  z-index: 1070;
  max-width: 550px;
  width: 100%;
  height: 200px;
  background-color: #fff;
  box-shadow: 0 10px 20px rgb(0 0 0 / 20%);
  opacity: 0;
  visibility: hidden;
  transition: all 0.75s ease;
  transform: translate3d(0, 100px, 0);
}

.popup-homepage .popup-container {
  width: 100%;
}

.popup-homepage .popup-container {
  height: 100%;
  box-sizing: border-box;
}

.popup-homepage.open .block-content-wrap {
  pointer-events: fill;
  width: 100%;
}

.popup-homepage .block-content-wrap {
  overflow: hidden;
  pointer-events: none;
}

.popup-homepage .columns {
  height: 100%;
  box-sizing: border-box;
}

.popup-homepage .close {
  position: absolute;
  right: 5px;
  top: 5px;
  transform: rotate(45deg);
  font-size: 20px;
  line-height: 1;
  cursor: pointer;
  z-index: 10;
}

.popup-homepage .close .icon {
  font-weight: 700;
}

.icon {
  font-family: icon !important;
  speak: none;
  font-style: normal;
  font-weight: 400;
  font-feature-settings: normal;
  font-variant: normal;
  text-transform: none;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-plus:before {
  content: '\e901';
}

.popup-homepage .picture {
  margin: 0;
  flex: 0 0 40%;
}

.popup-homepage .picture .wrap {
  padding: 10px;
}

.popup-homepage .picture img {
  height: 100%;
  width: 100%;
  -o-object-fit: cover;
  object-fit: cover;
}

.popup-homepage .entry .inner {
  padding: 25px 20px 25px 10px;
}

.popup-homepage .entry .section-headline {
  font-size: 14px;
  line-height: 26px;
  margin-bottom: 15px;
  letter-spacing: 2px;
  white-space: nowrap;
}

.section-headline.text-gold {
  color: #a67c07;
}

.section-headline {
  font: 400 35px/1.3 Playfair Display, serif;
  text-transform: uppercase;
  letter-spacing: 5px;
  color: #5f5c68;
  position: relative;
  margin-top: 0;
  display: block;
  margin-bottom: 50px;
}

.popup-homepage .entry .title {
  font-family: Playfair Display, serif;
  text-transform: uppercase;
  display: block;
  margin-bottom: 10px;
}

.popup-homepage .entry .desc {
  max-height: 40px;
  overflow: hidden;
  margin: 0 0 20px;
}

.popup-homepage .entry .button {
  display: flex;
  align-items: center;
  -webkit-align-items: center;
  text-transform: uppercase;
  font-size: 12px;
  line-height: 18px;
  display: inline-block;
}

.popup-homepage .entry .button .icon {
  border: 1px solid #679334;
  border-radius: 50%;
  width: 20px;
  height: 20px;
  display: inline-block;
  line-height: 1;
  margin-right: 25px;
  text-align: center;
  font-size: 18px;
  transition: all 0.3s ease;
}

.icon-angle-right:before {
  content: '';
}
</style>
