<template>
  <div class="home">
    <div><circle-loading /></div>
    <div><bubble-loading /></div>
    <div><teacup-loading /></div>
    <div><play-button /></div>
    <div><floating-button /></div>
    <div><progress-bar /></div>
  </div>
</template>

<script>
// @ is an alias to /src
import CircleLoading from "@/components/CircleLoading.vue";
import BubbleLoading from "@/components/BubbleLoading.vue";
import TeacupLoading from "@/components/TeacupLoading.vue";
import PlayButton from "@/components/PlayButton.vue";
import FloatingButton from "@/components/FloatingButton.vue";
import ProgressBar from "@/components/ProgressBar.vue";

export default {
  name: "home",
  components: {
    CircleLoading,
    BubbleLoading,
    TeacupLoading,
    PlayButton,
    FloatingButton,
    ProgressBar,
  }
};
</script>

<style>
.home {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(4, 1fr);
  justify-items: center;
  align-items: center;
  max-width: 800px;
  height: 100vh;
  margin: 0 auto;
}

.home > div {
  transform: scale(1.5);
}
</style>
