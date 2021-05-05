<template>
  <div class="browser" :class="{ '--black': blackMode }">
    <div class="browser__header">
      <div class="browser__action">
        <div></div>
        <div></div>
        <div></div>
      </div>
    </div>
    <div class="browser__body">
      <h1>International Moose Count Underway</h1>
      <p>
        The UN-sponsored International Moose Census got off to a flying start
        today with hopes for an increase in the worldwide moose population
        compared to last year’s disapointing figures. Among the traditional
        early reporters were Egypt, returning figures of six moose, a twenty
        percent increase on 2011’s figures of five, and Uruguay whose moose
        population remains stable at eleven.
        <br />
        Historically the only competitor to China in the far eastern moose
        markets has been Singapore but the tiny island nation is set to report a
        net loss, expecting a decrease of more than five percent on last year’s
        50,000 moose counted. The head of Singapore’s Agency for Agriculture,
        JingFeng Lau, explained to an incredulous Singaporean parliament
        yesterday that bad weather had contributed to this season’s poor
        showing, most notably when a cargo of 150 moose were swept out into the
        Indian ocean in a monsoon.
      </p>
    </div>
    <div class="browser__toggle">
      <input type="checkbox" id="checkbox" v-model="blackMode" />
      <label for="checkbox"></label>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      blackMode: false,
    };
  },
};
</script>

<style lang="scss"></style>
