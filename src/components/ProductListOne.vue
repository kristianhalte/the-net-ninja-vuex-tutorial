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
          <tr v-for="product in products">
            <td>{{ product.name }}</td>
            <td>$ {{ product.price }}</td>
          </tr>
        </tbody>
      </table>
    </section>
  </div>
</template>

<script>
export default {
  computed: {
    products() {
      return this.$store.state.products
    }
  }
}
</script>

<style>

</style>
