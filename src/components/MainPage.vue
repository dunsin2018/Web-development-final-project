<template>
  <div class="Main Page">
      Main page from component
      <ProductPanel title="Best offers"/> 
      <ProductPanel title="Latest Arrivals"/> 
      <ProductPanel title="On sales"/>

  </div>
</template>

<script>
import ProductPanel from "./ProductPanel.vue"
export default {
  name: 'MainPage',
  components: {
      ProductPanel,
    
  }
  
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.panel{
  border: 1px solid yellowgreen;
  padding: 10px;
  margin-bottom: 5px;
}
</style>
