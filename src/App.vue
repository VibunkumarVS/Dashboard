<template>
  <div class="app">
    <Sidebar />
    <div class="content">
      <Header />
      <div id="app">
        <MainContent />
      </div>
    </div>
      <AddItem />
  </div>
</template>

<script>
import Sidebar from "./components/Sidebar.vue";
import MainContent from "./components/MainContent.vue";
import Header from "./components/Header.vue";
import AddItem from "./components/AddItem.vue";

export default {
  name: "App",
  components: {
    Sidebar,
    MainContent,
    Header,
    AddItem,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat&display=swap");

.app {
  height: 100%;
  display: flex;
}

.content {
  width: 50%;
}

#app {
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
  display: flex;
  height: calc(100% - 50px);
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>
