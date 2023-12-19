<template>
     <div class="nav">
        <nav class="navbar">
          <div class="logo">
            <a href="index.html"><img src="assets/img/logo-sm.png" alt="Logo"></a>
          </div>
          <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="producten.html">Merch</a></li>
            <li><a href="login.html">Log in</a></li>
            <li><img src="assets/img/shoppingcart.png" alt="Shopping Cart"></li>
          </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'Navbar',
}
</script>

<style scoped>

.nav {
  background-color: #1C1C1C;
  width: 100%;
  position: inherit;
}
.nav .navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 10px;
}
.nav .navbar .logo {
  margin-left: 30px;
}
.nav .navbar .logo img {
  width: 60px;
  height: auto;
}
.nav .navbar .logo img:hover {
  opacity: 0.8;
  transition: 0.2s;
}
.nav .navbar .nav-links {
  list-style: none;
  display: flex;
  align-items: center;
}
.nav .navbar .nav-links li {
  margin-right: 50px;
}
.nav .navbar .nav-links li:hover {
  transform: translateY(-20%);
  transition: transform 0.2s ease-in-out;
}
.nav .navbar .nav-links li a {
  text-decoration: none;
  font-size: large;
  color: #E2E2E2;
  background-color: #EF3030;
  padding: 8px;
  border-radius: 5px;
}
.nav .navbar .nav-links li a:hover {
  text-decoration: none;
}
</style>