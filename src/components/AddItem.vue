<template>
    <div class="container">
    <form @submit.prevent="OnSubmit">
        <div class="radioButtons">
            <input type="radio" name="radio" value="income" checked/>
            <label for="income">Income</label>
            <input type="radio" name="radio" value="expense"/>
            <label for="expense">Expense</label>
        </div>
        <input type="number" class="inputElement" placeholder="Enter Amount"/>
        <input type="text" class="inputElement" placeholder="Enter Text"/>
        <button type="submit">Add</button>
    </form>
    </div>
</template>

<script>
export default {
    name: 'AddItem',
    methods: {
        OnSubmit(){
            console.log("Form Submitted");
        }
    }
}
</script>

<style scoped>

.radioButtons{
    text-align: space-around;
}
form{
    display:flex;
    flex-direction: column;
}
.container{
    width: 30%;
    height: 100%;
    background-color: darkmagenta;
    text-align: center;
    align-items: center;
    padding: 10px;
    box-sizing: border-box;
}
.inputElement{
    padding: 5px;
    width: 300px;
    border: 1px solid black;
    margin: 10px 0;
}

button{
    width: 100px;
    height: 30px;
}

input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}

/* Firefox */
input[type=number] {
  -moz-appearance: textfield;
}
</style>