<template>
  <div class="container">
    <div class="layer">
      <img src="../assets/night.jpg">
      <img src="../assets/night.jpg">
      <img src="../assets/night.jpg">
    </div>
  </div>
</template>

<style scope>
.container {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  width: 100%;
}

.layer {
  position: relative;
  background: rgba(0, 0, 0, 0.1);
  width: 190px;
  height: 329px;
  transform: rotate(-30deg) skew(25deg);
  transition: 0.5s;
}

.layer img {
  left: 0;
  position: absolute;
  width: 100%;
  transition: 0.5s;
}

.layer:hover img:nth-child(3) {
  transform: translate(30px, -30px);
  opacity: 1;
}
.layer:hover img:nth-child(2) {
  transform: translate(20px, -20px);
  opacity: 0.6;
}
.layer:hover img:nth-child(1) {
  transform: translate(10px, -10px);
  opacity: 0.2;
}
</style>