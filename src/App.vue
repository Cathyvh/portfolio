<template>
  <div id="app">
    <b-navbar fixed="top" id="nav">
      <!-- <div class="nav-name">
        <h1>Cathy van Heijst</h1>
        <h3>Front End Developer</h3>
      </div> -->
      <div class="nav-links">
        <a v-smooth-scroll class="link" href="#about">About</a>
        <a v-smooth-scroll class="link" href="#projects">Projects</a>
        <a v-smooth-scroll class="link" href="#contact">Contact</a>
      </div>
    </b-navbar>

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
body {
  background: rgb(255, 254, 252);
  background: linear-gradient(
    180deg,
    rgba(255, 254, 252, 1) 48%,
    rgba(250, 239, 226, 0.4598039899553571) 74%,
    rgba(226, 161, 91, 0.23571435410101538) 100%
  );
}
#app {
  font-family: "Lato", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #53847e;
  height: 100%;
  /* background-color: #fffefc;*/
}
#heading {
  text-align: center;
  padding-bottom: 3em;
  font-weight: bold;
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
  margin-top: ;
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
  padding-top: 2em;
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

@media (min-width: 799px) {
  #nav {
    padding: 20px 10px 5px 100px;
    display: flex;
    justify-content: flex-end;

    /* border-bottom: 5px dashed #e2a15b; */
  }
  .downArrow {
    margin: 20em auto 0 auto;
    align-items: flex-end;
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

.bounce {
  -moz-animation: bounce 3s infinite;
  -webkit-animation: bounce 3s infinite;
  animation: bounce 3s infinite;
}
@-moz-keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    -moz-transform: translateY(0);
    transform: translateY(0);
  }
  40% {
    -moz-transform: translateY(-30px);
    transform: translateY(-30px);
  }
  60% {
    -moz-transform: translateY(-15px);
    transform: translateY(-15px);
  }
}
@-webkit-keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  40% {
    -webkit-transform: translateY(-30px);
    transform: translateY(-30px);
  }
  60% {
    -webkit-transform: translateY(-15px);
    transform: translateY(-15px);
  }
}
@keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    -moz-transform: translateY(0);
    -ms-transform: translateY(0);
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  40% {
    -moz-transform: translateY(-30px);
    -ms-transform: translateY(-30px);
    -webkit-transform: translateY(-30px);
    transform: translateY(-30px);
  }
  60% {
    -moz-transform: translateY(-15px);
    -ms-transform: translateY(-15px);
    -webkit-transform: translateY(-15px);
    transform: translateY(-15px);
  }
}
</style>
