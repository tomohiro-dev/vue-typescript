<template>
  <button @click="onClick">MyButton</button>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Mybutton extends Vue {
  @Prop()
  public greet?: string;

  public onClick() {
    alert(this.greet);
  }
}
</script>
