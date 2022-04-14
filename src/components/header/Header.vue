<template>
  <header id="header">
    <router-link id="header-left" to="/">
      <div id="logo-container">
        <site-logo :logo-size="logoSize" />
      </div>
      <div class="page-title">Brainworx Shop</div>
    </router-link>
    <div id="header-right"></div>
  </header>
</template>

<script>
import SiteLogo from "@/components/header/SiteLogo.vue";

export default {
  name: "Header",
  components: {
    SiteLogo,
  },
  data: function () {
    return {
      logoSize: 50,
    };
  },
};
</script>

<style scoped>
#header {
  position: fixed;
  top: 0;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-items: flex-end;
  padding: 10px 0px;
  width: 100%;
  background: linear-gradient(90deg, #357590, #195369);
  box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.5);
}
#header-left {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  color: white;
}
#header-right {
  flex-grow: 1;
  display: flex;
  justify-content: center;
}
#logo-container {
  display: flex;
  align-content: center;
}
.page-title {
  text-align: left;
  line-height: 1;
  padding: 3px;
  font-size: 1.7em;
  font-weight: 700;
}
a {
  text-decoration: none;
}
@media (max-width: 988px) {
  #header {
    position: relative;
  }
  #header-left {
    justify-content: start;
    width: 100%;
  }
}
</style>
