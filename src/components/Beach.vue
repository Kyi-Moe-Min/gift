<template>
  <div class="animation-wrapper flex-center">
    <div class="wrapper">
      <img
        class="cloud"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_33.png"
      />
      <img
        class="sand"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_23.png"
      />
      <img
        class="wave"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_30.png"
      />
      <img
        class="umbrella"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_24.png"
      />
      <img
        class="livetube"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_25.png"
      />
      <img
        class="sun"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_27.png"
      />
      <img
        class="summer"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_28.png"
      />
      <img
        class="watermelon"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_29.png"
      />
      <img
        class="ball"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_31.png"
      />
      <img
        class="ballon"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_32.png"
      />
      <img
        class="drink"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_34.png"
      />
      <img
        class="rock"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_39.png"
      />
      <img
        class="starfish"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_40.png"
      />
      <img
        class="shell"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_41.png"
      />
      <img
        class="bikini"
        src="https://res-global.pfkml36.cn:11443/statics/live/common/gift/7_bikini_50.png"
      />
    </div>
  </div>
</template>

<style scoped>
/* duration is 4s */
.animation-wrapper {
  /* background-image: radial-gradient(
    circle,
    #fff 5%,
    #dff1fb 15%,
    #4fb8f3 50%,
    transparent
  ); */
  /* animation-name: none; */
  animation-name: fade-in;
  animation-duration: 4s;
  animation-fill-mode: forwards;
}
.animation-wrapper > div > img {
  position: absolute;
  animation-duration: 3s;
  animation-fill-mode: forwards;
}
.wrapper {
  position: relative;
  width: 100%;
  height: 100%;
  max-width: 600px;
  display: flex;
  justify-content: center;
  align-items: center;
  /* margin-top: 20%; */
}
.cloud {
  width: 100%;
  top: 16%;
  animation-name: cloud;
}
.sand {
  width: 100%;
  bottom: 34%;
}
.wave {
  width: 100%;
  bottom: 32%;
}
.sand,
.wave {
  animation-name: sand;
  animation-duration: 1.5s !important;
  animation-timing-function: cubic-bezier(0.76, 1.63, 0.68, 0.79);
}
.umbrella {
  width: 24%;
  right: 15%;
  transform: scale(0);
  animation-name: umbrella;
  animation-delay: 0.2s;
  transform-origin: left bottom;
}
.livetube {
  width: 14%;
  right: 13%;
  bottom: 41%;
  animation-name: lifetube;
  animation-duration: 0.5s !important;
}
.sun {
  width: 30%;
  left: 20%;
}
.summer {
  width: 69%;
  bottom: 38.6%;
  animation-name: summer;
  animation-duration: 1s !important;
  animation-timing-function: cubic-bezier(0.18, 1.87, 0.6, 0.66);
}
.ball {
  width: 10%;
  bottom: 35%;
  right: 27%;
  animation-name: ball;
}
.watermelon {
  width: 11%;
  right: 11%;
  bottom: 36%;
}
.drink {
  width: 7%;
  right: 6%;
  bottom: 37%;
  transform: scale(0);
  animation-delay: 0.2s;
}
.ballon {
  width: 15%;
  left: 10%;
  top: 37%;
  animation-name: ballon;
  animation-timing-function: linear;
}
.rock {
  left: 14%;
  width: 7%;
  bottom: 36%;
  animation-delay: 0.3s;
}
.starfish {
  left: 8%;
  width: 13%;
  bottom: 36%;
  animation-delay: 0.1s;
}
.shell {
  left: 9%;
  width: 5%;
  bottom: 36%;
  animation-delay: 0.2s;
}
.sun,
.watermelon,
.drink,
.rock,
.starfish,
.shell {
  transform: scale(0);
  transform-origin: center bottom;
  animation-name: drink;
  animation-duration: 1.5s !important;
}

.bikini {
  width: 50%;
  animation-name: bikini;
  animation-duration: 1.2s !important;
}

@media only screen and (min-width: 400px) {
  .cloud {
    top: 6%;
  }
  .sand {
    bottom: 20%;
  }
  .wave {
    bottom: 18%;
  }
  .umbrella {
    bottom: 32%;
  }
  .livetube {
    bottom: 31%;
  }
  .sun {
    bottom: 28%;
  }
  .summer {
    bottom: 27%;
  }
  .ball {
    bottom: 25%;
  }
  .watermelon {
    bottom: 26%;
  }
  .drink {
    bottom: 27%;
  }
  .ballon {
    top: 27%;
  }
  .rock,
  .starfish,
  .shell {
    bottom: 24%;
  }
}

@keyframes cloud {
  0% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(-10px, -10px);
  }
}
@keyframes sand {
  0% {
    transform: translateY(10px);
  }
  100% {
    transform: translateY(0);
  }
}
@keyframes umbrella {
  0% {
    transform: scale(0.5);
  }
  16% {
    transform: scale(1.075);
    animation-timing-function: ease-in-out;
  }
  32% {
    transform: scale(1);
    animation-timing-function: ease-in-out;
  }
  48% {
    transform: scale(1.05);
    animation-timing-function: ease-in-out;
  }
  64% {
    transform: scale(1);
    animation-timing-function: ease-in-out;
  }
  80% {
    transform: scale(1.025);
    animation-timing-function: ease-in-out;
  }
  96% {
    transform: scale(1);
    animation-timing-function: ease-in-out;
  }
  100% {
    transform: scale(1);
    animation-timing-function: ease-in-out;
  }
}
@keyframes lifetube {
  0% {
    transform: translate(17px, 13px);
  }
  100% {
    transform: translateY(0, 0);
  }
}
@keyframes sun {
  0% {
    transform: scale(0.5);
  }
  100% {
    transform: scale(1);
  }
}
@keyframes summer {
  0% {
    transform: translateY(-5px);
  }
  100% {
    transform: translateY(0);
  }
}
@keyframes ball {
  0% {
    transform: translateY(-7px);
  }
  25% {
    transform: translateY(-10px);
    animation-timing-function: ease-in-out;
  }
  50% {
    transform: translate(0, 0);
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
@keyframes drink {
  0% {
    transform: scale(0);
  }
  40% {
    transform: scale(1.05);
    animation-timing-function: ease-in-out;
  }
  60% {
    transform: scale(1);
    animation-timing-function: ease-in-out;
  }
  80% {
    transform: scale(1.02);
    animation-timing-function: ease-in-out;
  }
  100% {
    transform: scale(1);
    animation-timing-function: ease-in-out;
  }
}
@keyframes ballon {
  0% {
    transform: translate(10px, 20px);
    opacity: 0;
  }
  30% {
    opacity: 1;
  }
  70% {
    opacity: 1;
  }
  100% {
    transform: translate(-40px, -80px);
    opacity: 0;
  }
}
@keyframes bikini {
  0% {
    transform: rotate(90deg) scale(0);
  }
  30% {
    transform: rotate(-5deg) scale(1.05);
    animation-timing-function: ease-out;
  }
  45% {
    transform: rotate(4deg) scale(0.96);
    animation-timing-function: cubic-bezier(0.58, 0, 0.43, 1);
  }
  60% {
    transform: rotate(-4deg) scale(1.04);
    animation-timing-function: cubic-bezier(0.58, 0, 0.43, 1);
  }
  75% {
    transform: rotate(3deg) scale(0.97);
    animation-timing-function: cubic-bezier(0.58, 0, 0.43, 1);
  }
  90% {
    transform: rotate(-3deg) scale(1.03);
    animation-timing-function: cubic-bezier(0.58, 0, 0.43, 1);
  }
  100% {
    transform: rotate(0deg) scale(1);
    animation-timing-function: ease-in;
  }
}
@keyframes fade-in {
  0% {
    opacity: 0.5;
  }
  50% {
    opacity: 1;
    animation-timing-function: cubic-bezier(1, 0, 1, -0.12);
  }
  100% {
    opacity: 0;
  }
}
</style>
