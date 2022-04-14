<template>
  <div class="board">
    <div class="column" v-for="column of board" :key="column">
      <div class="coin" v-for="row of column" :key="row"></div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

var board = [
  [0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0],
];

export default defineComponent({
  name: "GameBoard",
  data() {
    return {
      board: board,
    };
  },
});
</script>

<style lang="scss" scoped>
.board {
  display: grid;
  grid-auto-flow: column;
  padding: 0.8rem;

  .coin {
    min-width: 2rem;
    min-height: 2rem;
    margin: 0.5rem 0.25rem;

    aspect-ratio: 1 / 1;

    background-color: #f4f4f4;
    border-radius: 50%;
  }
}
</style>
