<template>
  <div id="app">
    <a-layout>
      <Header />
      <a-layout-content>
        <!-- <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link> -->
        <router-view />
      </a-layout-content>
      <Footer />
    </a-layout>
  </div>
</template>

<script>
import Header from "./components/layout/header.vue";
import Footer from "./components/layout/footer.vue";

export default {
  components: { Header, Footer },
  setup() {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
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
