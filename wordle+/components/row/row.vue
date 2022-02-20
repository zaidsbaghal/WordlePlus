<template>
  <div class="row-container">
    <box id="boxThree"></box>
    <box id="boxTwo"></box>
    <box id="boxThree"></box>
    <box id="boxFour"></box>
    <box id="boxFive"></box>
  </div>
</template>

<script>
import box from "../box/box.vue";
export default {
  components: { box },
  setup() {},
};
</script>

<style scoped lang="scss">
.row-container {
  width: 100%;
  height: fit-content;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
</style>
