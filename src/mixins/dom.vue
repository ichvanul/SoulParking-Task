<script>
export default {
  methods: {
    showCart () {
      document.getElementById('food-cashier').classList.add('cart-on')
      document.querySelector('.trolly').classList.add('hidden')
      document.querySelector('nav').classList.add('cart-on')
      document.querySelector('.cart').classList.add('active')
    },
    hideCart () {
      document.getElementById('food-cashier').classList.remove('cart-on')
      document.querySelector('.trolly').classList.remove('hidden')
      document.querySelector('nav').classList.remove('cart-on')
      document.querySelector('.cart').classList.remove('active')
    }
  }
}
</script>
