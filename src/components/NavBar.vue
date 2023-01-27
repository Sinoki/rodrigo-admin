<template>
  <header>
    <div class="nav">
      <img src="@/assets/LogoRodrigoAdminhorizontal.png" class="img-logo" />

      <div class="menu" id="nav">
        <router-link to="/">(41)82418142</router-link> |
        <router-link to="/about">Sobre</router-link> |
        <router-link to="/services">Serviços</router-link> |
        <router-link to="/demonstration">Demonstração</router-link> |
        <router-link to="/contact">Contato</router-link> |
        <router-link to="/login">Login</router-link> |
        <router-link to="/boletos">2ª via Boletos</router-link>
      </div>
      <router-view />
    </div>
  </header>
  <body>
    <div class="background"></div>
  </body>
</template>

<script lang="ts">
export default {
  name: 'NavBar',
  components: {},
};
</script>

<style lang="scss" scoped>
@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

header {
  font-family: roboto, sans-serif;
}
.nav {
  height: 90px;
  width: 100%;
  background: #d2dae0;
}
.img-logo {
  width: 280px;
  height: 80px;
  margin-top: 5px;
  margin-left: 20px;
}

.menu {
  float: right;
  margin-right: 40px;
  margin-top: 10px;
}
.menu a {
  text-decoration: none;
  color: black;
  margin: 0 10px;
  line-height: 70px;
}
$color: #fff;

a:focus {
  color: #42b983;
  font-weight: bold;
  transition: 0.5s;
}

.background {
  background-position: center;
  background-size: cover;
  height: 100vh;
  background-image: url("../assets/buildings.jpg");
}

@media only screen and (max-width: 690px) {
  label {
    display: block;
    cursor: pointer;
  }
}
</style>
