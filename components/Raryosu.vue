<template>
  <div @click="clickRaryosu" class="raryosu">
    <img class="ryosu" src="~/assets/ryosu.png" />
    <img class="ra" src="~/assets/ra.png" />
  </div>
</template>
<script>
import { mapMutations } from 'vuex'

export default {
  methods: {
    clickRaryosu() {
      this.increment()
    },
    ...mapMutations({
      increment: 'increment'
    })
  }
}
</script>
<style>
.raryosu {
  position: relative;
  animation: 1s appear;
  width: 300px;
  height: 300px;
  cursor: pointer;
}

.ra {
  position: absolute;
  top: 0;
  left: 0;
  width: 300px;
  height: 300px;
}

.ryosu {
  animation: rr 30s linear infinite;
  position: absolute;
  top: 0;
  left: 0;
  width: 300px;
  height: 300px;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@keyframes rr {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(-360deg);
  }
}
</style>
