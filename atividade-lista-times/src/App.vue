<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="Home">
      <RouterLink to="/">Home</RouterLink>
    </div>
    <div class="Times">
      <RouterLink to="/Time">Time</RouterLink>
    </div>
    <div class="Jogadores">
      <RouterLink to="/about">Jogadores</RouterLink>
    </div>
  </header>
  <main>
    <RouterView />
  </main>
  <footer>rodape</footer>
</template>
<style>
header {
  border: 1px black solid;
  height: 15%;
  padding: 30px;
}
footer {
  border: 1px black solid;
}
main {
  height: 150vh;
}
.Jogadores {
  float: left;
  padding-left: 100px;
  padding-bottom: 0px;
}
.Times {
  float: left;
  padding-left: 70px;
}
.Home{
  float: left;
}
</style>
