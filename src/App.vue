<template>
  <div id="app">
    <div class="bg-gray-100">
      <div class="container mx-auto">
        <div class="flex flex-col justify-center items-center h-screen">
          <div class="text-4xl text-gray-700">Hello Vue2 + tailwindcss</div>
          <nav>
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link>
          </nav>
        </div>
      </div>
    </div>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
