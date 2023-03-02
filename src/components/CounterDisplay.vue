<template>
  <section class="countBox">
    <NavDisplay/>
     <div class="counter">
       <h1>Counter: {{ count }}</h1>
       <div class="input_wrap">
 
         <input type="number" v-model="inputValue" />
         <button @click="setValue(inputValue)" class="setValue">Set Value</button>
       </div>

       <div class="__btn">
         <button @click="increment">+</button>
         <button @click="decrement">-</button>
         <button @click="reset">Reset</button>
       </div>
     </div>
  </section>
  </template>
  
  <script>
 
  import useCounter from '@/composable/useCounter'
  import NavDisplay from './NavDisplay.vue';
  
  export default {
    setup() {
        const { count, increment, decrement, reset, setValue } = useCounter();
        return {
            count,
            increment,
            decrement,
            reset,
            setValue,
            inputValue: 0,
        };
    },
    components: { NavDisplay }
}
  </script>
  
  <style>
 .countBox{
  width: 100vw;
  height: 90vh;
  background-color: whitesmoke;
  clip-path: ellipse(100% 60% at 45% 38%);
 }
  .counter {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100%;
  }
  .input_wrap{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
  }
input[type = 'number']{
  outline: none;
  padding-left: 0.3rem;
  margin: 1rem 0;
  font-size: 25px;
  max-width: 350px;
  height: 60px;
  border: none;
  border-radius: 1rem;
}
.setValue{
  padding: 1rem;
  cursor: pointer;
  border: none;
  margin-left: 0.7rem;
  color: white;
  background-color: gray;
  font-size: 24px;
}
.setValue:hover{
  background-color: rgba(128, 128, 128, 0.588);
}
.__btn{
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  padding: 1rem;
}
.__btn button{
  width: 120px;
  height: 40px;
  border: none;
  margin: 1rem 0.7rem;
  border-radius: 10px;
  cursor: pointer;
  color: white;
  font-size: 20px;
  background-color: palevioletred;
}
.__btn button:hover{
  background-color: rgba(216, 112, 147, 0.604);
}
  
  </style>
  