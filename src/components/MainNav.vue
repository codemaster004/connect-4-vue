<template>
  <nav>
    <router-link to="/game-online">
      <div class="nav-box">
        <div class="icon"></div>
        <p>Online</p>
        <b>&#8250;</b>
      </div>
    </router-link>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainNav",
});
</script>

<style lang="scss" scoped>
@import "@/scss/variables.scss";

nav {
  margin-top: 2rem;

  a {
    text-decoration: none;
  }

  .nav-box {
    width: 90%;
    height: 5.5rem;
    padding: 0.5rem;
    margin: 0 auto;
    display: flex;
    align-items: center;

    background-color: #f2f2f2;
    border-radius: 0.7rem;

    color: $text-body-color;

    & > * {
      margin: 0 0.5rem;
    }

    .icon {
      width: 4rem;
      height: 4rem;
    }

    p {
      text-align: left;
      font-size: 1rem;
      font-weight: 500;
      line-height: 200%;
      flex-grow: 1;
    }

    b {
      width: 3rem;
      font-size: 1.3rem;
    }
  }
}
</style>
