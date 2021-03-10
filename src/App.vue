<template>
  <div id="app">
    <div id="nav">
      <div class="nav-name">
        <h1>Cathy van Heijst</h1>
        <h3>Front End Developer</h3>
      </div>
      <div class="nav-links">
        <router-link class="link" to="/">Home</router-link>
        <router-link class="link" to="/about">About</router-link>
        <router-link class="link" to="/contact">Contact</router-link>
      </div>
    </div>

    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link
      href="https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700;900&family=Mulish:wght@400;500;600;700&display=swap"
      rel="stylesheet"
    />
    <div class="router">
      <router-view />
    </div>
  </div>
</template>

<style>
html {
  background-color: #fffefc;
}
#app {
  font-family: "Lato", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #53847e;
  background-color: #fffefc;
}

h1,
h2,
h3,
h4 {
  font-family: "Mulish", sans-serif;
}

#nav a:hover {
  color: #e2a15b;
}

.nav-name {
  text-align: left;
  margin: 0;
  align-self: flex-end;
}
.nav-name h1 {
  margin-top: 20px;
  font-size: 60px;
  font-weight: 800;
}
.nav-name h2 {
  margin-bottom: 0;
}
.link {
  padding-right: 2em;
}
.nav-links {
  padding-top: 7em;
}
#nav a {
  font-weight: bold;
  font-size: 20px;
  text-decoration: none;
  color: #53847e;
}
a:visited {
  color: #53847e;
}
a {
  color: #53847e;
}
h2 {
  font-size: 32px;
}

#nav a.router-link-exact-active {
  color: #e2a15b;
}
.router {
  width: 70%;
  margin: 8.5em auto;
}
.button {
  background-color: #53847e;
  color: white;
  font-weight: bold;
  height: 3em;
  width: 10em;
  border: none;
  border-radius: 5px;
}
img {
  box-shadow: 3px 3px 8px -5px rgba(0, 0, 0, 0.59);
}
@media (min-width: 799px) {
  #nav {
    padding: 30px 100px;
    display: flex;
    justify-content: space-between;

    /* border-bottom: 5px dashed #e2a15b; */
  }
}

@media (max-width: 798px) {
  .router {
    width: 85%;
    margin: 5em auto 0 auto;
  }
  #nav {
    display: flex;
    flex-direction: column;
    margin: 1em auto;
    width: 85%;
  }
  .nav-name {
    text-align: left;
    margin: 0;
    align-self: flex-start;
  }
  .nav-name h1 {
    margin-top: 20px;
    font-size: 50px;
    font-weight: 800;
  }
  .nav-links {
    padding-top: 2em;
  }
}
</style>
