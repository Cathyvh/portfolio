<template>
  <div class="contact">
    <div class="form-container">
      <div class="form-text">
        <h2>Contact me</h2>
        <p>
          Thanks for checking my website! If any of this looked interesting,
          please reach out.
          <br />
          I'm looking for an intership from August the 30th to october the 22nd.
        </p>
        <p class="bold">You can reach me through:</p>
        <div class="links">
          <a href="mailto: cathyvheijst@gmail.com">Email</a>
          <a href="https://www.linkedin.com/in/cathy-van-heijst-87472b15a/">
            LinkedIn
          </a>
          <a href="https://github.com/Cathyvh"> GitHub</a>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.contact {
  height: 70vh;
  display: flex;
}
.form-container {
  padding-top: 10vh;
}

.links {
  display: flex;
  flex-direction: row;
  font-size: 20px;
  margin-top: 2em;
}

.links a {
  font-weight: bold;
  margin-bottom: 0.5em;
  color: #e2a15b;
  text-decoration: none;
  margin-right: 1em;
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