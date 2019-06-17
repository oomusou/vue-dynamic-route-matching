<template>
  <div>
    <h1>Products</h1>
    <h2>{{ product }}</h2>
  </div>
</template>

<script>
let products = {
  0: 'Shoes',
  1: 'T-Shirts',
  2: 'Pants',
};

let product = function() {
  return products[this.$route.query.id] || 'N/A';
};

export default {
  name: 'Products',
  computed: {
    product
  },
};
</script>
