<template>
  <header class="p-4">
    <div class="wrapper">
      <h1 class="font-semibold">Dynamic LTE Mobile Proxies</h1>
      <nav class="header-navigation">
        <ul class="d-flex list-navbar">
          <li><a href="#" class="navbar-link">Home</a></li>
          <li><a href="#" class="navbar-link">Prices</a></li>
          <li><a href="#" class="navbar-link">Contact</a></li>
          <li><a href="#" class="primary-btn">Sign Up</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.navbar-link {
  transition: all .3s ease;
}
.navbar-link:hover {
  color: #7064f5
}
.primary-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  border: 1px solid transparent;
  padding: 0.375rem 0.75rem;
  line-height: 1.5;
  background-color: #7064f5;
  box-shadow: 0px 5px 30px 0px #7b6ff67a;
  height: 46px;
  min-width: 165px;
  color: #ffffff;
  font-weight: 900;
  border-radius: 50px;
  transition: .3s ease-in-out;
}
.primary-btn:hover {
  background-color: #5c50d8;
  box-shadow: 0px 4px 20px 0px #6f64e270;
}
.list-navbar {
  display: flex;
  gap: 30px;
}
</style>
