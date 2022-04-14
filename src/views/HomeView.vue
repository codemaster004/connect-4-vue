<template>
  <div class="home">
    <MainHeader />
    <MainNav />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import MainHeader from "@/components/MainHeader.vue";
import MainNav from "@/components/MainNav.vue";

export default defineComponent({
  name: "HomeView",
  components: {
    MainHeader,
    MainNav,
  },
});
</script>
