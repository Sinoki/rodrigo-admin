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
        <router-link to="/boletos">2ª via Boletos</router-link> |
      </div>
      <router-view />
    </div>
  </header>
</template>

<script lang="ts">
export default {
  name: 'NavBar',
  components: {},
};
</script>

<style lang="scss" scoped>
@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");
* {
  text-decoration: none;
  list-style: none;
}
header {
  font-family: roboto, sans-serif;
  background-position: center;
  background-size: cover;
  height: 100vh;
}
.nav {
  height: 80px;
  width: 100%;
  background: #d2dae0;
}
.img-logo {
  width: 220px;
  height: 135px;
  padding-top: 20px;
  margin-top: -55px;
  margin-left: 20px;
  border: 2px solid black;
}

.menu {
  float: right;
  margin-right: 40px;
  margin-top: 5px;
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

@media only screen and (max-width: 690px) {
  label {
    display: block;
    cursor: pointer;
  }
}
</style>
