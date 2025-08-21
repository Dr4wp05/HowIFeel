<template>
  <div class="w-full h-[400px]">
    <Iridescence 
      :color="[1, 1, 1]"
      :speed="1.0"
      :amplitude="0.1"
      :mouseReact="true"
    />
  </div>

  <div class="fondo-completo">
    <VueBits class="fondo-absoluto" />
  </div>

</template>

<script setup lang="ts">
  import Iridescence from "./VueBits/Backgrounds/Iridescence.vue";
</script>

<style scoped>
.fondo-completo {
  position: relative;
  width: 100%;
  height: 100vh; /* altura completa de la ventana */
  margin: 0;
  padding: 0;
  overflow: hidden;
}

.fondo-absoluto {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>