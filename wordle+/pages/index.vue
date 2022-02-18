<template>
  <div class="wordle">
    <div class="header">
      <h1 class="title">Wordle+</h1>
    </div>
    <div class="matrix">
      {{ matrix }}
    </div>
    <div class="footer">
      <button class="restart-btn">Restart</button>
      <button class="new-word-btn">New Word</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dictionary: {},
      currentWord = "weary", // default word
      matrix: [
        [1, 2, 3, 4, 5],
        [1, 2, 3, 4, 5],
        [1, 2, 3, 4, 5],
        [1, 2, 3, 4, 5],
        [1, 2, 3, 4, 5],
        [1, 2, 3, 4, 5],
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.wordle {
  display: flex;
  flex-direction: column;
  height: 100vh;
  width: 100vw;
  .header {
    .title {
      width: 100%;
      display: flex;
      justify-content: center;
    }
  }
  .matrix {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .footer {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
}
</style>