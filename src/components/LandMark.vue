<template>
  <div class="land-mark"></div>
</template>

<style>
.land-mark {
  position: relative;
  display: flex;
  border-radius: 100%;
  width: 40px;
  height: 40px;
  filter: drop-shadow(0 1px 1px #973340a3);
  background-image: linear-gradient(0deg, red, #ff8484);
  animation: jump infinite 1.5s ease;
}
.land-mark::before {
  content: '';
  position: absolute;
  display: block;
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  width: 10px;
  height: 10px;
  background-color: red;
  transform: scaleX(1.5) translateY(2px) rotate(45deg);
}
.land-mark::after {
  content: '';
  position: absolute;
  display: block;
  top: 50%;
  left: 50%;
  margin-left: -5px;
  margin-top: -5px;
  border-radius: 100%;
  width: 10px;
  height: 10px;
  background-color: white;
  box-shadow: inset 0 1px 0 rgba(0, 0, 0, 0.4);
}
@keyframes jump {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-10px);
  }
  100% {
    transform: tranlateY(0px);
  }
}
</style>