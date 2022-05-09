<template>
  <nav>
    <router-link to="/">Here I say Hello</router-link> |
    <router-link to="/answer"
      >J'ai adoré le texte de votre annonce, elle méritait que je lui consacre
      quelques instants, cliquez pour voir ma réponse!</router-link
    >
    <router-link to="/me">Si j'ai su éveiller votre curiosité:</router-link>
  </nav>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
