<template>
  <div id="nav">
    <router-link to="/" id="logoURL">
      <img :src="logo" :alt="alt" id="logo">
    </router-link>
    <router-link to="/">Inicio</router-link>
    <router-link to="/pedidos">Pedidos</router-link>
  </div>
</template>

<script>
  export default{
    name: "Navbar",
    props:{
      logo: String,
      alt: String,
    }
  }
</script>

<style scoped>
  #nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }

  #nav #logoURL {
    margin: auto auto auto 0;
  }

  #logo {
    width: 40px;
    height: 40px;
  }

  #nav a {
    color: #FCBA03;
    text-decoration: none;
    margin: 12px;
    transition: .5s;
  }

  #nav a:hover {
    color: #fff;
  }
</style>