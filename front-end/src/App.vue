<template>
<div id="app">
  <div class="header">
    <router-link to="/">
      <div class="title">
        <h1>World's Greatest Supercar Dealership</h1>
      </div>
    </router-link>
    <div class="menu">
      <div class="menu-item">
        <router-link to="/contact">Contact</router-link>
      </div>
      <div class="menu-item">
        <router-link to="/admin">Admin</router-link>
      </div>
    </div>
  </div>
  <div class="content">
    <router-view />
  </div>
  <div class="footer">
  </div>
</div>
</template>

<style>
html {
  box-sizing: border-box;
}

body {
  font-family: 'Montserrat', sans-serif;
  font-size: 16px;
  background: #fff;
  padding: 0px;
  margin: 0px;
}

/* Header */
.header {
  display: flex;
  height: 100px;
  justify-content: space-between;
  align-items: center;
  background-color: black;
}

.title {
  margin-left: 50px;
}

.title h1 {
  font-size: 40px;
}

.menu {
  width: 300px;
  margin-right: 50px;
  display: flex;
  justify-content: space-around;
  font-size: 25px;
  font-weight: bold;
}

.content {
  padding: 20px 100px;
  min-height: 500px;
}

/* Footer */
.footer {
  height: 50px;
  padding: 20px 100px 0px 100px;
  background: #e3e3e3;
  font-size: 12px;
}

.footer a {
  color: #000;
}

h1 {
  font-size: 20px;
}

h2 {
  font-size: 14px;
}
</style>
