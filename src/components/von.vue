<template>
  <div>
    <h1>V-On</h1>
    <h2>{{ message }}</h2>
    <button v-on:click="add()" >Add</button>
  </div>
</template>


<script>
export default {
  data() {
    return {
      message: 0,
    };
  },

  methods : 
  {
    add() 
    {
      this.message = this.message + 1
    }
  }
};
</script>