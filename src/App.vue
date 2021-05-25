<template>
  <div class="app">
    <h1 class="h1">ISIMINK MANE</h1>
    <p>Spausk "START" isimink laukelius ir juos atspek</p>
  </div>

  <Board />
</template>

<script>
import Board from "./components/Board";

export default {
  name: "App",
  components: {
    Board,
  },
};
</script>

<style scoped>
.app {
  margin-top: 40px;
  text-align: center;
  font-family: "Quicksand", sans-serif;
}
</style>
