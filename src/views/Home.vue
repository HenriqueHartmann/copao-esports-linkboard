<template>
  <div class="card-style">
    <b-row class="header">
      <Header />
    </b-row>
    <b-row>
      <Links />
    </b-row>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import Links from "@/components/Links.vue";

export default {
  name: "Home",
  components: {
    Header,
    Links,
  },
};
</script>

<style scoped>
.card-style {
  width: 650px;
  margin: auto;
  padding: 0;
  padding-bottom: 5.5rem;
  background-color: #3c005a;
  height: 100vh;
}

.header {
  margin-bottom: 1.2rem !important;
}

@media only screen and (max-width: 950px) {
  .card-style {
    height: 100%;
  }
}

@media only screen and (max-width: 768px) {
  .card-style {
    height: 100%;
  }
}
</style>
