<template>
  <div
    class="keyboard__key"
    :class="keyClass"
    @click="playTone"
    data-key="dataKey"
  >
    {{ this.isBlack ? "" : note }}
  </div>
</template>

<script>
import * as Tone from "tone";
const synth = new Tone.Synth().toDestination();
// const now = Tone.now();

export default {
  props: {
    note: {
      type: String,
    },
    text: {
      type: String,
    },
    isBlack: {
      type: Boolean,
      default: false,
    },
  },
  methods: {
    playTone() {
      synth.triggerAttackRelease(this.note, 1);
    },
  },
  computed: {
    keyClass() {
      return this.isBlack ? "--black" : "--white";
    },
  },
};
</script>

<style></style>
