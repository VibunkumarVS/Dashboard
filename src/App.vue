<template>
<div class="app">
  <Header />
  <div id="app">
    <Sidebar />
    <MainContent />
    <AddItem/>
  </div>
</div>
</template>

<script>
import Sidebar from "./components/Sidebar.vue";
import MainContent from "./components/MainContent.vue";
import Header from "./components/Header.vue";
import AddItem from './components/AddItem.vue';

export default {
  name: "App",
  components: {
    Sidebar,
    MainContent,
    Header,
    AddItem
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat&display=swap");

.app{
    height: 100%;

}
#app {
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
  height: calc(100% - 50px);
  display: flex;
}

html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>
