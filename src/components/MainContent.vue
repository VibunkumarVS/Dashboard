<template>
  <div class="mainContent_Container">
    <div class="header">
    <div class='ulCont'>
      <ul>
        <li>All Transaction's</li>
        <li>Income</li>
        <li>Expense</li>
      </ul>
  </div>
      <div class="search_container">Search</div>
    </div>
    <MainBoard />
  </div>
</template>

<script>
import MainBoard from "./MainBoard.vue";

export default {
  name: "MainContent",
  components: {
    MainBoard,
  },
};
</script>

<style scoped>

@font-face {
    font-family: MarkPro;
    src: url("MARKPRO.OTF") format("opentype");
}

.mainContent_Container {
  height: 100%;
  box-sizing: border-box;
  width: 100%;
  padding: 5px 50px;
font-family:MarkPro

}

.ulCont{
  width: 350px;
  display: inline-block;
  font-size: 16px;
    font-weight: 600;

  color: blue;
}


ul {
  list-style: none;
  display: flex;
  justify-content: space-between;
  margin: 0;
  padding: 0 0 10px 0;

}


li {
  display: inline-block;
}

.header {
  width: 100%;
  margin: 20px 0;
  display: inline-block;
  border-bottom : solid 0.5px grey;
}

.search_container {
  float: right;
  margin-right: 30px;
}
</style>