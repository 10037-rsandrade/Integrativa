<template>
  <div id="app">
    <user-list-component></user-list-component>
  </div>
</template>

<script>
import UserListComponent from './UserListComponent.vue';

export default {
  components: {
    UserListComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
