<template>
  <div class="contact">
    <div class="form-container">
      <div class="form-text">
        <h2>Contact me!</h2>
        <p>
          Does all of this look interesting? In that case, please reach out. I
          am looking for in intership at the moment and anything Front End would
          be of interest.
        </p>
        <p class="bold">You can also find me at:</p>
        <div class="links">
          <a href="https://www.linkedin.com/in/cathy-van-heijst-87472b15a/">
            LinkedIn
          </a>
          <p class="amp">&#38;</p>
          <a href="https://github.com/Cathyvh"> GitHub</a>
        </div>
      </div>
      <form name="contact" method="POST" netlify="true">
        <label for="name">Name</label>
        <input name="name" class="input" type="text" />
        <label for="email">Email Address</label>
        <input name="email" class="input" type="email" />
        <label for="messsage">Message</label>
        <textarea name="message" id=""></textarea>
        <input name="button" class="button" type="submit" value="Submit" />
      </form>
    </div>
  </div>
</template>
<style scoped>
.contact {
  height: 100vh;
  display: flex;
}
.form-container {
  padding-top: 20vh;
}

.links {
  display: flex;
  flex-direction: row;
  font-size: 20px;
  margin-top: 2em;
}
.amp,
.links a {
  font-weight: bold;
  margin-bottom: 0.5em;
  color: #e2a15b;
  text-decoration: none;
}
.amp {
  margin: 0 0.5em;
  color: #53847e;
}
.bold {
  font-weight: 600;
}
@media (min-width: 1101px) {
  .form-container {
    display: flex;
    flex-direction: row-reverse;
    justify-content: center;
  }

  form {
    display: flex;
    flex-direction: column;
    padding-right: 5em;
  }
  label {
    font-weight: bold;
  }
  .input {
    width: 40em;
    height: 2em;
    margin: 0.7em 0 2em 0;
  }
  textarea {
    width: 40em;
    height: 9em;
    resize: none;
    margin: 0.7em 0 1em 0;
  }
}
@media (max-width: 1100px) {
  .form-text {
    padding-bottom: 2em;
  }
  .form-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  form {
    display: flex;
    flex-direction: column;
  }
  label {
    font-weight: bold;
  }
  .input {
    width: 90%;
    height: 2em;
    margin: 0 0 1.5em 0;
  }
  textarea {
    width: 90%;
    height: 7em;
    resize: none;
    margin: 0.7em 0 1em 0;
  }
  .button {
    margin-bottom: 3em;
  }
}
</style>