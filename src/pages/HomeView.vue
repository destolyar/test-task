<template>
  <nav class="home-router">
    <RouterLink class="home-router__link" to="/login">Login</RouterLink>
    <RouterLink class="home-router__link" to="/registration">Registration</RouterLink>
  </nav>
</template>


<style>
  .home-router {
    width: 300px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .home-router__link {
    font-size: 20px;
    text-decoration: none;
    color: black;
  }  
</style>