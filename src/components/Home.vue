<template>
  <div class="container align-center full-height p-0 m-0">
    <div id="canvas-p5"></div>
    <div class="pt-3 col-sm-6 col-md-2 mx-auto">
      <img class="img-fluid logo" src="../assets/hypercube-symbol.svg"/>
    </div>
    <vue-particles class="particles"
    color="#033860"
    :particleOpacity="0.7"
    :particlesNumber="20"
    shapeType="circle"
    :particleSize="4"
    linesColor="#033860"
    :linesWidth="1"
    :lineLinked="true"
    :lineOpacity="0.4"
    :linesDistance="300"
    :moveSpeed="3"
    :hoverEffect="true"
    hoverMode="grab"
    :clickEffect="true"
    clickMode="push"
    ></vue-particles>
    <div class="center-of-page">
      <h2 class="m-0">#Be</h2>
      <h2 class="m-0">Digital</h2>
    </div>
    <a href="mailto:contato@hypercube.br"><h5 class="footer">contato@hypercube.be</h5></a>
  </div>
</template>

<script>
export default {
  name: 'Home',

  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1  {
  font-weight: normal;
}
h2 {
  font-weight: 300;
  font-size: 1000%;
  color: #00918F;
}
@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  h2 {
    font-size: 600%;
  }
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #033860;
}

.full-height {
  width: 100vw;
  height: 100vh;
  background: linear-gradient(to bottom, #D5DEE7 0%, #E8EBF2 50%, #E2E7ED 100%), linear-gradient(to bottom, rgba(0,0,0,0.02) 50%, rgba(255,255,255,0.02) 61%, rgba(0,0,0,0.02) 73%), linear-gradient(33deg, rgba(255,255,255,0.20) 0%, rgba(0,0,0,0.20) 100%);
  background-blend-mode: normal,color-burn;
}

.center-of-page {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.particles {
  height: 100vh;
  width: 100vw;
  position: absolute;
}

.footer {
  font-family: 'Lato', Helvetica, Arial, sans-serif;
  left: 50%;
  transform: translate(-50%);
  bottom: 20px;
  position: fixed;
  vertical-align: bottom;
}

.logo {
  max-width: 180px;
}
</style>
