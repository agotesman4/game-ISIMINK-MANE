<template>
  <div class="wrapper">
    <BoardItem v-for="i in 25" :key="'item-' + i" />
  </div>
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
  width: 320px;
  height: 100px;
  background: #eee;
  margin: 0 auto;
}
</style>
