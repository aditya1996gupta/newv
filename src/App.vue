<template>
  <div id="app">
    <message v-if="showMsg" msg="Vue Lifecycle Hooks"></message>
    <button @click="showMsg = false">Hide</button>
  </div>
</template>

<script>
import Message from "./components/Message.vue";
export default {
  name: "app",
  components: {
    Message
  },
  data() {
    return {
      showMsg: true
    };
  }
};
</script>
<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
