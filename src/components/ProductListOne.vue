<template>
  <div id="product-list-one">
    <h2>Product List One</h2>
    <ul>
      <li v-for="product in products">
        <span>{{ product.name }}</span>
        <span>$ {{ product.price }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ['products']
}
</script>

<style>

</style>
