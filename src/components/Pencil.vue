<template>
  <div class="pencil">
    <div class="pencil__tip"></div>
    <div class="pencil__top"></div>
    <div class="pencil__crayon">
      <div class="pencil__crayon --left"></div>
      <div class="pencil__crayon --center"></div>
      <div class="pencil__crayon --right"></div>
    </div>
    <div class="pencil__metal"></div>
    <div class="pencil__rubber"></div>
    <div class="pencil__circle"></div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HelloWorld",
  props: {
    msg: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// .pencil {
//   background: red;
//   height: 50px;
// }
</style>
