<template>
  <div class="mb-2">
    <b-img :src="logo" class="logo"></b-img>
    <b-jumbotron
    class="jumbotron-style"
    >
    <template #header><h1 class="j-header">{{ header }}</h1></template>
    <template #lead><p class="j-lead">{{ lead }}</p></template>
    </b-jumbotron>
  </div>
</template>

<script>
export default {
  name: "Header",
    data() {
    return {
      logo: require("../assets/logo/logo.png"),
      header: 'COPÃO',
      lead: 'Links para formulários e redes sociais. Youtube e Twitch para acompanhar os jogos e Discord para contato e mais informações.'
    };
  },
};
</script>

<style>
  @font-face {
  font-family: "Kenyan Coffee";
  src: local("Kenyan Coffee"), url(../assets/fonts/kenyan_coffee_rg.ttf) format("truetype");
  }

  @font-face {
  font-family: "Inter";
  src: local("Inter"), url(../assets/fonts/Inter.ttf) format("truetype");
}

  .logo {
    width: 100px;
  }

 .jumbotron-style {
  width: 450px;
  margin: auto;
  padding: 0;
  color: white
 }

 .jumbotron-style .j-header {
  font-family: 'Kenyan Coffee', sans-serif;
  font-weight: 400;
  font-size: 5rem;
  letter-spacing: 0.3rem;
 }

.jumbotron-style .j-lead {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1.3rem;
 }
</style>
