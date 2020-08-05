<template>
  <div id="app">
    <Header />
    <Navegation />
    <Articles :posts="posts" />
    <SideBar />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Navegation from "./components/Navegation.vue";
import Articles from "./components/Articles.vue";
import SideBar from "./components/SideBar";

export default {
  name: "App",
  components: {
    Header,
    Navegation,
    Articles,
    SideBar,
  },
  data() {
    return {
      posts: [
        { content: "Text 1" },
        { content: "Text 2" },
        { content: "Text 3" },
        { content: "Text 4" },
      ],
    };
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
}
</style>
