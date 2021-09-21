<template>
  <div id="start">
    <div class="start-content">
      <h1>Hello!</h1>
      <h1>I'm Cathy van Heijst</h1>
      <h2>A Front End Developer student, looking for my next challenge</h2>
      <div class="downArrow bounce">
        <a v-smooth-scroll href="#about">
          <svg
            width="40"
            viewBox="0 0 180 238"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M89.9997 237.763C86.7737 237.763 83.5482 236.528 81.0887 234.064L3.69255 156.481C-1.23085 151.546 -1.23085 143.544 3.69255 138.611C8.61396 133.678 16.5948 133.678 21.5186 138.611L89.9997 207.261L158.481 138.613C163.405 133.68 171.385 133.68 176.306 138.613C181.231 143.546 181.231 151.548 176.306 156.483L98.9107 234.066C96.45 236.531 93.2245 237.763 89.9997 237.763Z"
              fill="#E2A15B"
            />
            <line
              x1="12.5"
              y1="-12.5"
              x2="193.723"
              y2="-12.5"
              transform="matrix(0.0097423 0.999953 -0.999952 0.00976898 75.271 1)"
              stroke="#E2A15B"
              stroke-width="25"
              stroke-linecap="round"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>
<style scoped>
@media (min-width: 801px) and (max-width: 1250px) {
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
@media (min-width: 1250px) {
  .downArrow {
    margin: 15em auto 0 auto;
    align-items: flex-end;
  }
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