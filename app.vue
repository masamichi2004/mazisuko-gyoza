<template>
  <div class="app">
    <img src="@/public/img/mazisuko.jpg" width="100%" />

    <div class="dumplings">
      🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟
    </div>

    <div class="center-text">
      <p>水餃子が1杯無料で食べられるクーポンです🎉この画面を店員に提示してください🙇</p>
    </div>

    <div class="dumplings bottom-line">
      🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟🥟
    </div>
  </div>
</template>

<style>
body {
  margin: 0;
  overflow: hidden;
  background: #f7f7f7;
}

.app {
  position: relative;
  width: 100vw;
  height: 100vh;
}

img {
  display: block;
  width: 100%;
}

.dumplings {
  white-space: nowrap;
  font-size: 2rem;
  position: absolute;
  left: 0;
  transform: translateY(-50%);
  animation: scroll infinite linear 30s;
}

.top-line {
  top: calc(100% - 50px);
}

.bottom-line {
  bottom: 0;
}

.center-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  background-color: rgba(255, 255, 255, 0.8);
  padding: 20px;
  border-radius: 10px;
  font-size: 1.5rem;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}

@keyframes scroll {
  0% {
    transform: translateX(-100%);
  }
  100% {
    transform: translateX(100vw);
  }
}
</style>
