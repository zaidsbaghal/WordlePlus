<template>
  <div class="wordle">
    <div class="header">
      <h1 class="title">Wordle+</h1>
    </div>
    <div class="matrix">
      <row></row>
      <row></row>
      <row></row>
      <row></row>
      <row></row>
    </div>
    <div class="footer">
      <button class="reset-btn">Reset Board</button>
      <button class="new-word-btn">New Word</button>
    </div>
  </div>
</template>

<script>
import row from "../components/row/row.vue";
export default {
  components: { row },
  data() {
    return {
      dictionary: {},
      currentWord: "", // default word
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
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .footer {
    margin: 25px;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    .restart-btn {
      margin: 10px;
    }
    .new-word-btn {
      margin: 10px;
    }
  }
}
</style>