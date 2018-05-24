<template>
  <div id="app">
    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column">
            <product-list-one v-bind:products="products"></product-list-one>
          </div>
          <div class="column">
            <product-list-two :products="products"></product-list-two>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ProductListOne from './components/ProductListOne';
import ProductListTwo from './components/ProductListTwo';
export default {
  components: {
    'product-list-one': ProductListOne,
    ProductListTwo
  },
  name: 'app',
  data () {
    return {
      products: [
        { name: 'Banana Skin', price: 20 },
        { name: 'Shiny Star', price: 40 },
        { name: 'Green Shells', price: 60 },
        { name: 'Red Shells', price: 80 }
      ]
    }
  }
}
</script>

<style>

</style>
