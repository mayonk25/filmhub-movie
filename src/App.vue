<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lato:wght@700&display=swap" rel="stylesheet">
    <RouterLink to="/">
      <h1><span>Film</span>HUB</h1>
    </RouterLink>
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans&display=swap');
*{
  margin: 0;
  padding : 0;
  box-sizing: border-box;
  font-family: 'Nunito Sans', sans-serif;

  &::selection{
    background: transparentize(#42B883, 0.5);
  }
}
body{
  background-color: #35495e;
}
a{
  text-decoration: none;
}
header{
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background-color: #2c3d4e;
  box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.2);

  h1{
    color :rgb(255, 106, 0);
    font-size: 28px;
  }
  span{
    color: white;
  }
}
</style>
