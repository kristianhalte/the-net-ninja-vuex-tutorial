<template>
  <div id="product-list-one">
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            Product List One
          </h1>
        </div>
      </div>
    </section>
    <section class="section">
      <table class="table">
        <thead>
          <tr>
            <th>Product</th>
            <th>Price</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="product in saleProducts">
            <td>{{ product.name }}</td>
            <td>$ {{ product.price }}</td>
          </tr>
        </tbody>
      </table>
    </section>
    <section class="section">
      <a class="button" @click="reducePrice(4)">Reduce Price</a>
      <a class="button" @click="increasePrice(2)">Increase Price</a>
    </section>
  </div>
</template>

<script>
import { mapActions, mapGetters } from 'vuex'
export default {
  computed: {
    products() {
      return this.$store.state.products
    },
    ...mapGetters([
        'saleProducts'
      ])
  },
  methods: {
    ...mapActions([
        'reducePrice',
        'increasePrice'
      ])
  }
}
</script>

<style>

</style>
