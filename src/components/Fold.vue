<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Fold",
  data() {
    return {};
  },
  methods: {},
});
</script>

<template>
  <section class="fold">
    <img src="../assets/brand/logo1.png" alt="Portal Shop" />
    <div class="text">
      <h1>Portal Shop</h1>
      <h3>Twój portal do marzeń!</h3>
    </div>
  </section>
</template>

<style scoped lang="scss">
@import "../assets/main.scss";

.fold {
  width: 100vw;
  height: 86vh;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  animation: appear 0.6s ease-in;
}
img {
  width: 26rem;
  height: 26rem;
}

h1 {
  color: $dark-purple;
  padding-bottom: 2rem;
  font-size: 4rem;
}

h3 {
  color: $light-purple;
  font-size: 2rem;
}

@media (max-width: 1100px) {
  img {
    display: none;
  }
}

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
