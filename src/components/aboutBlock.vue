  
  <template>
  <div class="about">
    <div class="about-box">
      <div class="about-text">
        <h2>About me!</h2>
        <p>
        With a past in Customer Success, I'm now diving headfirst into Front End Development.
        <br>Learning as much as I can about development, agile workflows, UX and design.
        <br> <br/>
        My passion lies in startups and companies that contribute in making our society a better place, either through environmental or humanitarian means. 
        <br>I have a past in a tech-startup which has given me a great foundation for future work in IT and a good knowledge of the growing pains of a startup.
        <br><br />
          Besides that, I am creative, curious and I also like to think that I'm funny.
        </p>
      </div>
      <div class="about-img"><img src="../assets/img/profil.png" alt="" /></div>
    </div>
  </div>
</template>
<style scoped>
.about {
  height: 80vh;
  display: flex;
  align-content: center;
  padding-top: 20vh;
  margin: 0 auto;
}
@media (min-width: 801px) {
  img {
    width: 25em;
  }
  .about-text {
    max-width: 40em;
    margin-right: 3em;
  }
  .about-box {
    display: flex;
    text-align: left;
    margin: 1em auto;
    justify-content: space-around;
  }
}
@media (max-width: 800px) {
  .about {
    height: 100%;
  }
  .about-box {
    display: flex;
    flex-direction: column;
    text-align: left;
    margin: 5em 0;
  }
  .about-img {
    display: flex;
    justify-content: center;
  }
  img {
    width: 70%;
    margin: 2em 0;
    border-radius: 7px;
  }
}
</style>