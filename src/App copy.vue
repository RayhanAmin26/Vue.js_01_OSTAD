<script setup>

import {ref} from 'vue';
const country = "Bangladesh"
const capital = "Dhaka"


// const count = ref(0);
const time = "morning"

const countries = ref([
{ name: "United States", capital: "Washington, D.C." },
        { name: "Canada", capital: "Ottawa" },
        { name: "United Kingdom", capital: "London" },
        { name: "France", capital: "Paris" },
        { name: "Germany", capital: "Berlin" },
        { name: "Australia", capital: "Canberra" },
        { name: "India", capital: "New Delhi" },
        { name: "Japan", capital: "Tokyo" },
        { name: "China", capital: "Beijing" },
        { name: "Brazil", capital: "Brasília" },
]);

// function greet(){
//   alert("Hello")
// }
// const increment = () => {
//   count.value+= 5;
// };

</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <!-- <h1 v-if="time=='morning'">Good Morning</h1>
      <h1 v-else-if="time=='afternoon'">Good Afternoon</h1>
      <h1 v-else>Good Evening</h1>
      <p>It is a beautiful day in {{ country }}.The capital city is {{ capital }}.</p> -->

      <h1>Countries with capital</h1>
      <ul>
        <li v-for="country in countries":key="country.name">
          {{ country.name }} - {{ country.capital }}
        </li>
      </ul>

      <ul>
        <li v-for="country in countries":key="country.name">
          {{index+1}}. {{ country.name }} - {{ country.capital }}
        </li>
      </ul>
    </div>








      <!-- <h1>welcome to {{ country }} - {{ count }}</h1> -->
      <!-- <p> -->
       <!-- The capital is {{ capital }}.<button @click="greet()">Greet</button> -->
        <!-- The number is {{ count }} -->
      <!-- </p> -->
      <!-- <p>
        <button @click="increment()">Increment</button>
        <button @click="incrementBy5()">Increment5</button>
      </p>
       -->
    
  </header>

  <main>
    
   
  </main>
</template>

<style scoped>

</style>
