<template>
  <div id="product-list-two">
    <h2>Product List Two</h2>
    <ul>
      <li v-for="product in products">
        <span v-text="product.name"></span>
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
