<template>
  <div class="app">
    <h1 class="h1">ISIMINK MANE</h1>
    <p>Spausk "START" isimink laukelius ir juos atspek</p>

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
.logo {
  width: 100px;
}
</style>
