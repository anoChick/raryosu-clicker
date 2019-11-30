<template>
  <div class="raryosu-counter">
    <span>{{ raryosuCount }} らりょす</span>
  </div>
</template>
<script>
export default {
  computed: {
    raryosuCount() {
      return this.$store.state.raryosuCount
    }
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
</style>
