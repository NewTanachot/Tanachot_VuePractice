<template>
  <div>
    <h1>V-Bind</h1>
    <button
      v-bind:class="{ green: check, blue: !check }"
      v-on:click="check = !check"
    />
    <h1 v-if="check">This is TRUE</h1>
    <h1 v-else >This is FALSE</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      check: true,
    };
  },
};
</script>

<style>
.green {
  background-color: green;
  width: 100px;
  height: 100px;
}
.blue {
  background-color: blue;
  width: 100px;
  height: 100px;
}
</style>