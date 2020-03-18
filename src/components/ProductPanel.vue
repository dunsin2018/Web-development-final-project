<template>
  <div class="product-panel">  
    <h3>{{ title }}</h3>

    <b-card-group deck>
    <ProductCard 
    :product="product" 
    v-for="product in products" 
    :key="product.id"/>
    </b-card-group>
  </div>
  
</template>

<script>
import ProductCard from './ProductCard.vue'

export default {
  name: 'ProductPanel',
  props:{
      title: String
  },
  components: {
      ProductCard
  },
  data(){
      return{
          products: []
      };
  },
  mounted(){
      this.products = [{
          id:1,
          title:'Card Title1',
          image: "/imagesforvue/try1.jpeg",
          description:'some quick example text to build on the card'
      },
       {  id:2,
          title:'Card Title2',
          image:"/imagesforvue/try2.jpeg",
          description:'some quick example text to build on the card'

      }]
  }
  
  }
</script>

<style scoped>
.product-panel{
    border: 1px solid red;
    margin-bottom: 15px
}

</style>
