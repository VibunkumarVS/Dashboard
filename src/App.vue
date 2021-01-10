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
import Sidebar from "./components/Sidebar/Sidebar.vue";
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
@import url('https://fonts.googleapis.com/css2?family=Nunito&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Mulish&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');


@font-face {
    font-family: MarkPro;
    src: url("assets/fonts/MARKPRO.OTF") format("opentype");
}

 .app {
font-family:MarkPro;
  height: 100%;
  display: flex;
}

.content {
  width: 55%;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>
