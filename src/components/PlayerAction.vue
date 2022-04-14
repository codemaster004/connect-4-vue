<template>
  <div>
    <div class="icon-box"></div>
    <p>Reset</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "PlayerAction",
});
</script>

<style lang="scss" scoped>
.icon-box {
  width: 3.9rem;
  height: 3.9rem;
  margin: 0 auto 1rem;

  background-color: #eee;
  border-radius: 50%;

  font-size: 1.6rem;
  font-weight: 500;
  line-height: 3.9rem;
  text-align: center;
}
p {
  display: inline-block;
  font-size: 1.4rem;
}
</style>
