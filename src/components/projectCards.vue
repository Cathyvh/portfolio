<template>
  <div>
    <div class="cards-gallery">
      <h2 id="heading">Projects</h2>

      <div class="cards img-right">
        <img src="../assets/img/airbean.jpg" alt="" />
        <div class="cards-text">
          <h2>Airbean</h2>
          <p>
            Airbean - Dronedelivered coffee
            Built an API storing the menu and prices and accounts with a lowDB database.
            I built the the rest of the app using <strong>react, redux, redux store and lowDB</strong>, we had to follow a finished design by the school.
          </p>
          <div class="links link">
            <a
              href="https://github.com/Cathyvh/airbean-project"
              >GitHub</a
            >
          </div>
        </div>
      </div>
      <div class="cards img-left">
        <img src="../assets/img/neo.png" alt="" />
        <div class="cards-text">
          <h2>Near Earth Objects</h2>
          <p>
            A PWA project made in Vue.js Fetching data from the NASA JPL
            Asteroid team. Using Vuex, Bootsrap Vue and and Nasas API i built
            this responsive website where you can search for near earth objects
            on a specific date.
          </p>
          <div class="links link">
            <a
              href="https://github.com/Cathyvh/Near-Earth-Obejct-Vue.js-project"
              >GitHub</a
            >
            <a href="https://cathys-vue-project.netlify.app/#/">Visit me!</a>
          </div>
        </div>
      </div>
      <div class="cards img-right">
        <img src="../assets/img/sinus.png" alt="" />
        <div class="cards-text">
          <h2>Sinus webshop</h2>
          <p>
            During our UX-course we had an assignment to design a webshop for a
            made up skater brand in Figma.
          </p>
        </div>
      </div>
      <div class="cards img-left">
        <img src="../assets/img/tarot.png" alt="" />
        <div class="cards-text">
          <h2>Tarot Reading</h2>
          <p>
            Our first Nativ Javascript assignment, using only a CSS, HTML and JS
            file. I fetched data from a
            <a href="https://github.com/ekelen/tarot-api">tarot-API</a>. You can
            pick cards just like a real tarot reading and click on the cards for
            description and meaning.
          </p>
          <div class="links link">
            <a href="https://github.com/Cathyvh/Tarot-project">GitHub</a>
          </div>
        </div>
      </div>
      <div class="cards img-right">
        <img src="../assets/img/kvinnofrid.png" alt="" />
        <div class="cards-text">
          <h2>KvinnoFrid</h2>
          <p>
            My very first school assignment. We had to build a website using
            only HTML and CSS for a made up organisation. I chose a helpline for
            women. Semantic code and readability was very important for me, also
            a button to easily leave the website if needed.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "projectCards",
  props: {},
};
</script>
<style scoped>
.links {
  display: flex;
  flex-direction: row;
}
#heading {
  text-align: center;
}
img {
  box-shadow: 3px 3px 8px -5px rgba(0, 0, 0, 0.59);
}
.cards-text .link a {
  font-weight: 700;
  color: #e2a15b;
  margin-bottom: 0.7;
  margin-right: 1em;
  text-decoration: none;
}
.cards-text a {
  font-weight: 700;
  color: #e2a15b;
 text-decoration: none;
}
.cards-text a:hover {
  color: #53847e;
}
@media (min-width: 1101px) {
  .cards {
    display: flex;
    margin-bottom: 15em;
    text-align: left;
  }
  img {
    width: 55%;
    border-radius: 7px;
  }
  .cards-text {
    padding: 1em 2.5em;
    width: 45%;
  }
  .img-right {
    display: flex;
    flex-direction: row;
  }
  .img-right {
    display: flex;
    flex-direction: row-reverse;
  }
  .cards-gallery {
    padding-top: 20vh;
  }
}
@media (max-width: 1100px) {
  .cards-gallery {
    display: flex;
    flex-direction: column;
    padding-top: 20vh;
  }
  .cards {
    width: 100%;
    display: flex;
    margin: 2.5em 0;
    text-align: left;
  }
  img {
    border-radius: 7px;
  }
  .cards-text {
    padding-top: 2em;
  }
  .img-right,
  .img-left {
    display: flex;
    flex-direction: column;
  }
}
</style>