<template lang="pug">
  div(id="app" class="mt-5")
    shop-layout
      template(slot="product-list")
          product-list
      template(slot="cart")
          cart
</template>

<script>
import ShopLayout from '@/components/ShopLayout'
import ProductList from '@/components/ProductList'
import Cart from '@/components/Cart'

export default {
  name: 'app',
  components: {
    ShopLayout, ProductList, Cart
  }
}
</script>
<style lang="stylus">
#app
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px
</style>
