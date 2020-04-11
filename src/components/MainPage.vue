<template>
  <div class="Main Page">
    Main page from component
    <ProductPanel title="Recommended" section="recommended" />

    <ProductPanel title="BuyNow" section="buynow" />

    <ProductPanel title="TopSelling" section="topselling" />
  </div>
</template>

<script>
import ProductPanel from "./ProductPanel.vue";
export default {
  name: "MainPage",
  components: {
    ProductPanel
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
