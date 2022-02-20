<template>
  <div class="box-container">
    <div class="letter-box">
      <input
        class="text-box"
        type="text"
        maxlength="1"
        autocapitalize="on"
        :disabled="disableBox"
      />
    </div>
  </div>
</template>

<script>
export default {
  setup() {},
  data() {
    return {
      disableBox: false
    };
  },
};
</script>

<style scoped lang="scss">
.box-container {
  background-color: lightgray;
  height: 60px;
  width: 60px;
  margin: 10px;
  .letter-box {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    .text-box {
      background-color: lightgray;
      height: 60px;
      width: 60px;
      border: none;
      text-align: center;
      caret-color: transparent;
      text-transform:uppercase;
    }
  }
}
</style>
