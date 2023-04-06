<script>
import { def, slotFlagsText } from "@vue/shared";

export default {
  data() {
    return {
      count: 0,
    };
  },
  components: { slotFlagsText },
};
</script>

<template>
  <button class="button" @click="count++">Count {{ count }}</button>
  <slot></slot>
  <slot name="description"></slot>
  <button @click="count = 0">
    <slot name="button-text"></slot>
  </button>
</template>

<style>
.button {
  border: 1px solid lightgray;
  box-shadow: 1px 1px 20px lightgrey;
  font-weight: bold;
  color: black;
  background-color: white;
}
</style>
