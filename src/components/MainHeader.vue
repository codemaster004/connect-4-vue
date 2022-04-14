<template>
  <header>
    <img alt="Vue logo" src="../assets/logo.png" />
    <h1>Lets Connect 4</h1>
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainHeader",
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/scss/variables.scss";
h1 {
  font-size: 2rem;
  color: $primary-color;
  margin: 10px 0;
}
img {
  height: 70px;
}
</style>
