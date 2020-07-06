<template>
  <div id="food-cashier">
    <div>
      <Navbar @modal-clicked="showModal"
              @cart-clicked="showCart" />
      <Cart @cart-clicked="hideCart"
            @cancel-clicked="cancelOrder"
            @checkout-clicked="showModalCheckout" />
      <Footer/>
    </div>
    <router-view/>
  </div>
</template>

<script>
import Navbar from '@/components/base/Navbar.vue'
import Cart from '@/components/base/Cart.vue'
import Footer from './components/base/Footer.vue'
import dom from '@/mixins/dom.vue'

export default {
  mixins: [dom],
  components: {
    Navbar,
    Cart,
    Footer
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_reset.scss';
@import '@/assets/scss/_font.scss';
body {
  background-color: rgb(247, 247, 247);
}
#food-cashier {
  font-family: 'Airbnb Cereal App', Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000;
  transition: .3s;
  &.cart-on {
    margin-left: 25vw;
  }
}
</style>
