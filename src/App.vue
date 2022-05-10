<template>
  <nav>
    <router-link to="/"
      ><div class="routerLink">Here I say Hello</div></router-link
    >

    <router-link to="/answer"
      ><div class="routerLink">
        J'ai adoré le texte de votre annonce, elle méritait que je lui consacre
        quelques instants, cliquez pour voir ma réponse!
      </div></router-link
    >

    <router-link to="/me">
      <div class="routerLink">
        Si j'ai su éveiller votre curiosité:
      </div></router-link
    >
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
  width: 55%;
  padding: 1.5rem;
  display: flex;
  text-align: left;
  justify-content: space-evenly;
  margin: auto;
  background-color: #d23b38;
}

nav a {
  font-weight: bold;
  color: black;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: white;
  background-color: black;
}
.routerLink {
  padding: 0.5rem;
}
</style>
