<template>
  <div id="app">
    <navbar />
    <router-view />
    <link-chatbot-widget ref="chatbot" />
  </div>
</template>

<script>
export default {
  name: "App",
  mounted() {
    this.$refs.chatbot.shadowRoot.querySelector('div').querySelector('div').style['min-height'] = 0;
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  background-color: white;
}

body {
  margin: 0;
}
</style>
