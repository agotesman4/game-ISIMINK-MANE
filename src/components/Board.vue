<template>
  <div class="board-wrapper">
    <div class="board">
      <BoardItem v-for="i in 25" :key="'item-' + i" />
    </div>

    <div class="play">
      <p class="difficult">
        Lygis: <strong>{{ difficult }}</strong>
      </p>
      <button class="btn">START</button>
    </div>
  </div>
</template>

<script>
import BoardItem from "./BoardItem";
import { ref } from "vue";

export default {
  name: "Board",
  props: {},
  components: {
    BoardItem,
  },
  setup() {
    const difficult = ref(3);

    return {
      difficult,
    };
  },
};
</script>

<style scoped>
.board-wrapper {
  margin-bottom: 100px;
}

.board {
  width: 300px;
  background: #eee;
  margin: 0 auto;
}

.play {
  margin: 0 auto;
  text-align: center;
  width: 300px;
}

.btn {
  background: #42b983cc;
  color: white;
  border: none;
  border-radius: 2px;
  padding: 10px 30px;
  margin: 10px 0;
  cursor: pointer;
  outline: none;
}

button:hover {
  background: #42b983;
}
</style>
