<template>
  <div>
    <button class="btn btn-primary" @click="asyncIncrement({ by: 20, duration: 750 })">Increment</button>
    <button class="btn btn-primary" @click="asyncDecrement({ by: 20, duration: 750 })">Decrement</button>
  </div>
</template>

<script>
import { mapActions } from "vuex";

export default {
  methods: mapActions(["asyncIncrement", "asyncDecrement"])
};
</script>