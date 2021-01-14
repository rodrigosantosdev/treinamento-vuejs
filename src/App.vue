<template>
  <div id="wrapper">
    <div id="nav">
      <router-link class="nav-item" to="/">Home</router-link>
      <router-link class="nav-item" to="/about">About</router-link>
      <router-link class="nav-item" to="/diretivas">Diretivas</router-link>
    </div>
    <div id="main">
      <router-view/>  
    </div>
  </div>
</template>

<style scoped>

  #wrapper {
    display: flex;
    justify-content: space-between;
  }

  #nav {
    width: 150px;
    height: 100vh;
    display: flex;
    flex-direction: column;
    background: var(--primary);
    padding: 10px;
  }

  .nav-item {
    font-size: 18px;
    text-transform: uppercase;
    padding: 10px 0;
  }

  #main {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top: 20px;
   }
</style>