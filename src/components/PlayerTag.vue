<template>
  <div class="playerTag">
    <div class="points-box">0</div>
    <p>Player 0</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "PlayerTag",
});
</script>

<style lang="scss">
.playerTag {
  width: 37%;
  // height: 6rem;
  max-width: 30rem;
  border-radius: 0.7rem;
  text-align: left;
  align-items: center;
  padding: 0.8rem;
  display: flex;

  .points-box {
    width: 3.9rem;
    height: 3.9rem;
    margin-right: 1.5rem;

    background-color: #f2f2f2;
    border-radius: 50%;

    font-size: 1.6rem;
    font-weight: 500;
    line-height: 3.9rem;
    text-align: center;
  }

  p {
    font-size: 1.6rem;
    font-weight: 500;
  }
}
</style>
