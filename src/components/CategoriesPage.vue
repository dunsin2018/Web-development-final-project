<template>
  <div class="category-page">
    categories for {{ this.$route.params.categoryAlias }}
    <ProductPanel :categoryAlias="this.$route.params.categoryAlias" />
  </div>
</template>

<script>
import ProductPanel from "./ProductPanel.vue";
export default {
  name: "CategoriesPage",
  components: {
    ProductPanel
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>