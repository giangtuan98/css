<template>
  <div class="neumorphic">
    <div class="rings">
      <div class="ring --first"></div>
      <div class="ring --second"></div>
      <div class="ring --third"></div>
      <div class="ring --fourth"></div>
      <!-- <div class="ring --fifth"></div> -->
    </div>

    <div class="pick-color">
      <div class="color" @click="handleChangeRingColor('red')"></div>
      <div class="color --green" @click="handleChangeRingColor('green')"></div>
      <div class="color --blue" @click="handleChangeRingColor('blue')"></div>
      <div
        class="color --purple"
        @click="handleChangeRingColor('purple')"
      ></div>
      <div
        class="color --yellow"
        @click="handleChangeRingColor('yellow')"
      ></div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  methods: {
    handleChangeRingColor(color: string) {
      document.documentElement.style.setProperty("--ring-color", color);
    },
  },
})
export default class Neumorphic extends Vue {}
</script>

<style></style>
