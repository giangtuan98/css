<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <KeyBoard />
  <ThemeToggle />
  <Neummorphic />
  <Pencil />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import KeyBoard from "./components/KeyBoard.vue";
import Neummorphic from "./components/Neummorphic.vue";
import ThemeToggle from "./components/ThemeToggle.vue";
import Pencil from "./components/Pencil.vue";

@Options({
  components: {
    KeyBoard,
    Neummorphic,
    Pencil,
    ThemeToggle,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
