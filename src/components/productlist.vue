<template>
    <div>
      <Product v-for="product in products" :key="product.id" :product="product" />
    </div>
  </template>
  
  <script>
  import Product from './Product.vue';
  
  export default {
    components: {
      Product,
    },
    data() {
      return {
        products: [
          { id: 1, name: 'Product 1', description: 'Description for Product 1', price: 10 },
          { id: 2, name: 'Product 2', description: 'Description for Product 2', price: 20 },
          // More products...
        ],
      };
    },
  };
  </script>