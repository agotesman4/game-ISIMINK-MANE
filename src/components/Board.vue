<template>
  <div class="wrapper">
    <BoardItem v-for="i in 25" :key="'item-' + i" />
  </div>

  <p class="difficult">Lygis: <strong>3</strong></p>

  <button>START</button>
</template>

<script>
import BoardItem from "./BoardItem";

export default {
  name: "Board",
  props: {},
  components: { BoardItem },
};
</script>

<style scoped>
.wrapper {
  width: 300px;
  background: #eee;
  margin: 0 auto;
}
</style>
