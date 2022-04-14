<template>
  <div id="app-body">
    <Footer />
    <router-view />
    <Header />
  </div>
</template>

<script>
import Header from "@/components/header/Header.vue";
import Footer from "@/components/footer/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
body {
  margin: 0px;
}
#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #28667f;
  margin: 0px;
}
#app-body {
  display: flex;
  flex-direction: column-reverse;
  min-height: 100vh;
}
#body {
  margin-top: 100px;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  overflow: hidden;
}
@media (max-width: 988px) {
  #body {
    margin-top: 0px;
  }
}
.section {
  width: 1100px;
  margin: 0px auto;
}
#page {
  flex-grow: 1;
  background-color: white;
}
</style>
