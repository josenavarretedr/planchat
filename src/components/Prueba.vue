<template>
  <div>
    <h1>Hola desde Prueba!</h1>
    <p class="message">{{ message }}</p>
    <div class="divPrueba">HOLA</div>
  </div>
</template>

<script>
export default {
  name: "Prueba",
  setup() {
    return {
      // data
    };
  },
};
</script>

<style lang="scss">
.message {
  color: red;
}

.divPrueba {
  width: 80%;
  @include util.breakpoint("sm") {
    background: cyan;
  }

  @include util.breakpoint("md") {
    background: blue;
  }

  @include util.breakpoint("lg") {
    background: green;
  }

  @include util.breakpoint("xl") {
    background: yellow;
  }
}
</style>
