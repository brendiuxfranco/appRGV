<template>
  <div id="app">
    <div class="min-h-screen bg-green-900">
      <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/register">Registration</router-link> |
        <router-link to="/calendar">Calendar 2020</router-link> |
        <router-link to="/about">About RGV League</router-link> |
        <router-link to="/contacts">Contact Us</router-link> 
      </div>
      <router-view />
      <div class="flex justify-center items-center">
        <div class="h-20 bottom-o py-9 flex">
          <p class="pr-2">&copy; RGV League APP</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #01070c;
  background: seagreen;
}

#nav {
  padding: 70px;

  a {
    font-weight: bold;
    color: #fa0b0b;

    &.router-link-exact-active {
      color: rgb(68, 85, 70);
    }
  }
}
</style>
