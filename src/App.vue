<template>
  <div id="app">
    <p class="wording">視力検査</p>
    <div class="alph-v left"></div>
    <div class="alph-v right"></div>
    <div class="alphabet alph-s">S</div>
    <div class="alph-i"></div>
    <div class="alph-a left"></div>
    <div class="alph-a right"></div>
    <div class="alph-a-lighter left"></div>
    <div class="alph-a-lighter right"></div>
    <div class="visual">visual</div>
    <div class="acuity">acuity</div>
    <div class="_1213">12 / 13</div>
    <div class="_1215">12 / 15</div>
    <div class="alph-i-light"></div>
    <div class="alph-l"></div>
    <div class="gestalt-girl">ゲシュタルト乙女</div>
    <div class="alph-t top"></div>
    <div class="alph-t bottom"></div>
    <div class="alph-y left"></div>
    <div class="alph-y right"></div>
    <div class="alph-y bottom"></div>
    <div class="alph-u"></div>
    <div class="alph-u-light"></div>
    <div class="alph-s-light"></div>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {
  }
}
</script>

<style lang="scss">

$orange: #D2422A;
$orange-light: #DC7765;
$orange-lighter: #E9BFB3;

html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  font-family: 'Noto Serif JP', serif;
  display: flex;
  justify-content: center;
  align-items: center;
}

#app {
  width: 595px;
  height: 545px;
  background: #F2F3EE;
  position: relative;
  overflow: hidden;
  .gestalt-girl {
    font-family: 'Noto Serif JP', serif;
    font-size: 13px;
    color: #D3402C;
    position: absolute;
    top: 275px;
    left: 375px;
    transform: rotate(90deg);
    letter-spacing: 5px;
  }
  .wording {
    color: #235298;
    letter-spacing: 1.5rem;
    font-size: 1.5rem;
    position: absolute;
    top: 45%;
    left: 45%;
    transform: translate(-50%, -50%);
  }
  .visual {
    font-family: 'Noto Serif TC', serif;
    font-size: 12px;
    letter-spacing: 1px;
    color: #EEC1BC;
    writing-mode: vertical-rl;
    position: absolute;
    top: 165px;
    left: 107px;
  }
  .acuity {
    font-family: 'Noto Serif TC', serif;
    font-size: 12px;
    letter-spacing: 1px;
    color: #D9775E;
    position: absolute;
    left: 216px;
    top: 343px;
  }
  ._1213 {
    color: #DF7565;
    font-size: 12px;
    position: absolute;
    left: 220px;
    top: 110px;
  }
  ._1215 {
    color: #DF7565;
    font-size: 12px;
    position: absolute;
    left: 358px;
    bottom: 96px;
  }
  .alph-s-light {
    position: absolute;
    width: 27px;
    height: 30px;
    left: 295px;
    top: 305px;
    transform: rotate(90deg);
    border: 15px solid $orange-lighter;
    border-bottom: 15px solid $orange-lighter;
    border-top: none;
    border-right: none;
    border-bottom-left-radius: 35px;
  }
  .alph-l {
    position: absolute;
    width: 27px;
    height: 46px;
    left: 406px;
    top: 123px;
    border: 18px solid #DC7765;
    border-bottom: 14px solid #DC7765;
    border-top: none;
    border-right: none;
  }
  .alph-u {
    position: absolute;
    width: 30px;
    height: 52px;
    left: 404px;
    bottom: 121px;
    border: 18px solid #DC7765;
    border-bottom: 18px solid #DC7765;
    border-top: none;
    border-right: none;
    border-bottom-left-radius: 34px;
  }
  .alph-u-light {
    position: absolute;
    width: 23px;
    height: 40px;
    left: 104px;
    top: 225px;
    border: 15px solid $orange-lighter;
    border-bottom: 15px solid $orange-lighter;
    border-top: none;
    border-right: none;
    border-bottom-left-radius: 24px;
  }
  .alph-t {
    position: absolute;
    background: $orange-light;
    &.top {
      width: 70px;
      height: 15px;
      bottom: 97px;
      left: 269px;
    }
    &.bottom {
      width: 18px;
      height: 60px;
      bottom: 48px;
      left: 295px;
    }
  }
  .alph-v {
    position: absolute;
    top: -25px;
    background: $orange;
    &.left {
      width: 48px;
      height: 150px;
      transform: skew(27deg);
      left: 70px;
    }
    &.right {
      width: 48px;
      height: 150px;
      transform: skew(-27deg);
      left: 146px;
    }
  }
  .alph-y {
    position: absolute;
    background: $orange;
    &.left {
      width: 40px;
      height: 80px;
      transform: skew(35deg);
      right: 44px;
      bottom: 32px;
    }
    &.right {
      width: 40px;
      height: 80px;
      transform: skew(-35deg);
      right: -12px;
      bottom: 32px;
    }
    &.bottom {
      width: 40px;
      height: 40px;
      right: 16px;
      bottom: 0;
    }
  }
  .alph-i {
    position: absolute;
    background: $orange;
    left: -5px;
    bottom: 0;
    width: 48px;
    height: 110px;
  }
  .alph-i-light {
    position: absolute;
    background: #DC7765;
    left: 304px;
    top: 72px;
    width: 19px;
    height: 54px;
  }
  .alph-a {
    position: absolute;
    background: $orange-light;
    bottom: 115px;
    &.left {
      width: 28px;
      height: 80px;
      transform: skew(23deg);
      left: 160px;
    }
    &.right {
      width: 28px;
      height: 80px;
      transform: skew(-23deg);
      left: 127px;
    }
  }
  .alph-a-lighter {
    position: absolute;
    background: $orange-lighter;
    top: 180px;
    &.left {
      width: 15px;
      height: 44px;
      transform: skew(23deg);
      left: 314px;
    }
    &.right {
      width: 15px;
      height: 44px;
      transform: skew(-23deg);
      left: 296px;
    }
  }
  .alphabet {
    &.alph-s {
      font-family: 'Noto Sans', sans-serif;
      font-family: 'Hind Madurai', sans-serif;
      font-size: 18rem;
      color: $orange;
      position: absolute;
      top: -70px;
      right: -62px;
    }
  }
}
</style>
