<template>
  <div>
    <div class="players">
      <PlayerTag />
      <PlayerTag />
    </div>
    <GameBoard />
    <div class="actions">
      <PlayerAction />
      <PlayerAction />
      <PlayerAction />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import GameBoard from "@/components/GameBoard.vue";
import PlayerTag from "@/components/PlayerTag.vue";
import PlayerAction from "@/components/PlayerAction.vue";

export default defineComponent({
  name: "GameOnline",
  components: {
    GameBoard,
    PlayerTag,
    PlayerAction,
  },
});
</script>

<style lang="scss" scoped>
.players {
  display: flex;
  justify-content: space-evenly;
  margin: 2rem 0 4rem;
}
.actions {
  margin-top: 5rem;
  display: flex;
  justify-content: space-evenly;
}
</style>
