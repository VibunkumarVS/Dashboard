<template>
  <div class="container">
    <!-- <form @submit.prevent="OnSubmit">
        <div class="radioButtons">
            <input type="radio" name="radio" value="income" checked/>
            <label for="income">Income</label>
            <input type="radio" name="radio" value="expense"/>
            <label for="expense">Expense</label>
        </div>
        <input type="number" class="inputElement" placeholder="Enter Amount"/>
        <input type="text" class="inputElement" placeholder="Enter Text"/>
        <button type="submit">Add</button>
    </form> -->
    <div class="header">
      <img class="icon" src="../assets/logo.png" />
      <h3>Sale Title</h3>
      <h2><strong> $ 1,400.10 </strong></h2>
    </div>

    <div class="bottom">
      <label>Balance</label>
      <div class="balance">$ 1,875.13</div>

      <div class="footer">
          <!-- <div class="text">Total Amount $ 1500.34 is for 2 months
              </div> -->
          </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AddItem",
  methods: {
    OnSubmit() {
      console.log("Form Submitted");
    },
  },
};
</script>

<style scoped>

label{
    font-size: 12px;
    margin-bottom: 20px;
    box-sizing: border-box;
}

.header {
  padding-bottom: 30px;
  border-bottom: 0.3px solid rgb(201, 201, 201);
  text-align: center;
}
.icon {
  width: 100px;
  height: 100px;
}

.footer {
position: absolute;
width: calc(30% - 100px);
box-sizing: border-box;
bottom: 20px;
  color: black;
}

.text{
    margin: 0 50px;
    padding: 5px 0;
    border-radius: 15px;
    border: 1px solid black;
    text-align: center;
}

.balance {
  font-size: 20px;
  margin-top: 5px;
}

.bottom {
  margin-top: 50px;
}

.radioButtons {
  text-align: space-around;
}
form {
  display: flex;
  flex-direction: column;
}
.container {
  /* border-left: 0.3px solid rgb(201, 201, 201); */
  background-color: #f5f8f9;
  width: 30%;
  height: 100%;
  padding: 0 30px;
  box-sizing: border-box;
  padding: 100px 50px;
}
.inputElement {
  padding: 5px;
  width: 300px;
  border: 1px solid black;
  margin: 10px 0;
}

button {
  width: 100px;
  height: 30px;
}

input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}

/* Firefox */
input[type="number"] {
  -moz-appearance: textfield;
}
</style>