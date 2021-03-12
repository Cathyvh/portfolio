<template>
  <div id="start">
    <div class="start-content">
      <h1>Hello!</h1>

      <h1>I'm Cathy van Heijst</h1>
      <h2>A Front End Developer student looking for an intership</h2>
      <div class="downArrow bounce">
        <a v-smooth-scroll href="#about">
          <img
            width="50
          "
            height="60"
            alt=""
            src="data:image/svg+xml;base64,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"
          />
        </a>
      </div>
    </div>
  </div>
</template>
<style scoped>
@media (min-width: 801px) and (max-width: 1200px) {
  #start {
    height: 80vh;
    display: flex;
  }
  .downArrow {
    margin: 5em auto;
  }
  .start-content {
    display: flex;
    flex-direction: column;
    text-align: left;
    padding-top: 4em;
    margin: 0 auto;
  }
  h1 {
    font-size: 97px;
  }
}
@media (min-width: 1201px) {
  #start {
    height: 80vh;
    display: flex;
  }
  .start-content {
    display: flex;
    flex-direction: column;
    text-align: left;
    padding-top: 8em;
    margin: 0 auto;
  }
  h1 {
    font-size: 97px;
  }
}

@media (max-width: 800px) {
  #start {
    height: 100vh;
  }
  .start-content {
    padding-top: 4em;
    display: flex;
    flex-direction: column;
  }
  .downArrow {
    margin: 6em auto;
  }
  h1 {
    font-size: 60px;
  }
}
</style>