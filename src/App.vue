
<!-- Se coloca la logica -->
<script setup>
const name = "Este es un vue dinamico";
const arrayFrutas = [
        {
            name: "Manzana",
            price: "$1.00",
            description: "Una manzana",
        },
        {
            name: "Pera",
            price: "$2.00",
            description: "Una pera",
        },
        {
            name: "Naranja",
            price: "$3.00",
            description: "Una naranja",
        },
    ];
// const arrayFrutas = ["🍎", "🍌", "🍉", "🍓", "🍒"];
// const styleColor = "color:pink";
// const arrayColores = ["blue", "red", "Alix"];
// const activo = true;
</script>


<!-- Estructura -->
<template>
  <h1>Hola vue 🦉 {{ name.toUpperCase() }}</h1>
  <ul>
    <li v-for:="(name,index) in arrayFrutas" key="index">{{name.name}}-{{name.price}}-{{name.description}}</li>
  </ul>

  <!-- <h2>{{ arrayColores }}</h2>
  <h2 :style="`color:${arrayColores[2]}`">Soy azul 😀</h2>
  <br />
  <h2 :style="styleColor">Soy Rosa :)</h2>
  <br />
  <h2 v-if="activo">1. Estoy activo</h2>
  <p v-else-if="activo === false">2. Estoy inactivo</p>
  <p v-else>3. Estoy indeciso</p>

  <h2 v-show="activo">Este codigo funciona v-show</h2> -->
</template>

<!-- Se coloca el estilo -->
<style>
h1 {
  color: rgb(104, 182, 196);
}
</style>