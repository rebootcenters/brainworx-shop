<template>
  <div id="shop">
    <div id="coming-soon">
      <div>Coming Soon!</div>
      <div>
        In the meantime, please email info@rebootcenters.org with your request.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Shop",
  components: {},
};
</script>

<style scoped>
#shop {
  flex-grow: 1;
  margin-top: 80px;
}
#coming-soon {
  font-size: 3em;
  text-align: center;
  padding: 30px;
}
@media (max-width: 988px) {
  #shop {
    margin-top: 0px;
  }
}
</style>
