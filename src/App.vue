<template>
  <div id="app">
    <router-link class="link" :to="{ path: '/' }">Home</router-link>
    <router-link class="link" :to="{ path: '/vmodel' }">V-Model</router-link>
    <router-link class="link" :to="{ path: '/von' }">V-On</router-link>
    <router-link class="link" :to="{ path: '/vbind' }">V-Bind</router-link>
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
#app {
  margin: 60px;
  text-align: center;
}
.link {
  display: inline-block;
  padding: 10px;
  text-decoration: none;
  color: inherit;
}
.router-link-exact-active {
  color: blue;
}
</style>
