<template>
  <div>
    <b-nav vertical>
      <b-nav-item
        v-for="category in categories"
        :key="category.alias"
        :to="'/categories/' + category.alias"
      >{{category.title}}</b-nav-item>
    </b-nav>
  </div>
</template>ß

<script>
import axios from "axios";
export default {
  name: "CategoriesMenu",
  data: function() {
    return {
      categories: []
    };
  },
  mounted() {
    axios.get("euas.person.ee/categories").then(response => {
      this.categories = response.data;
    });
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
