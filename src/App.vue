<template>
  <div id="app">
    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column">
            <product-list-one></product-list-one>
          </div>
          <div class="column">
            <product-list-two></product-list-two>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ProductListOne from './components/ProductListOne'
import ProductListTwo from './components/ProductListTwo'
export default {
  components: {
    'product-list-one': ProductListOne,
    ProductListTwo
  },
  name: 'app',
  data () {
    return {
      
    }
  }
}
</script>

<style>

</style>
