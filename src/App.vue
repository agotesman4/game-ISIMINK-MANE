<template>
  <div class="app">
    <h1 class="h1">ĮSIMINK MANE</h1>
    <p>Spausk "START" įsimink laukelius ir juos atspėk</p>

    <Board />
  </div>
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
  font-family: "Quicksand", sans-serif;
  text-align: center;
  margin-top: 40px;
}
</style>
