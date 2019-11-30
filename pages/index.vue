<template>
  <div class="container">
    <div>
      <Raryosu />
      <RaryosuCounter />
    </div>
  </div>
</template>

<script>
import Raryosu from '~/components/Raryosu.vue'
import RaryosuCounter from '~/components/RaryosuCounter.vue'

export default {
  components: {
    Raryosu,
    RaryosuCounter
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
