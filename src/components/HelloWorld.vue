<template>
  <div class="hello">
    <button class="1foo-button mdc-button">Button</button>
    <br />
    <br />

    <button class="bar-button mdc-button" data-mdc-auto-init="MDCRipple">
      <i class="material-icons mdc-button__icon" aria-hidden="true">favorite</i>
      Favorite
    </button>
    <br />
    <br />

    <button class="button0 mdc-button mdc-button--dense">
      <i class="material-icons mdc-button__icon" aria-hidden="true">edit</i>
      Dense button
    </button>
    <br />
    <br />

    <button class="button1 mdc-button mdc-button--unelevated" data-mdc-auto-init="MDCRipple">
      Unelevated
    </button>

    <br />
    <br />

    <button class="button2 mdc-button mdc-button--outlined" data-mdc-auto-init="MDCRipple">
      <i class="material-icons mdc-button__icon" aria-hidden="true">save</i>
      Outline
    </button>

    <br />
    <br />


    <button class="button3 mdc-button mdc-button--raised" data-mdc-auto-init="MDCRipple">
      <i class="material-icons mdc-button__icon" aria-hidden="true">sync</i>
      Raised
    </button>
  </div>
</template>

<script lang="ts">

import Vue from 'vue';
import { ripple, autoInit } from 'material-components-web';

export default Vue.extend({
  name: 'HelloWorld',
  mounted: () => {
    const secondButton: any = document.querySelector('.mdc-button');
    autoInit();
    // ripple.MDCRipple.attachTo(secondButton);
  },
  props: {  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
