<template>
  <nav>
    <div>
      <button class="burger">
        <img src="@/assets/img/menu.png">
      </button>
      <div>
        <button class="search">
          <img src="@/assets/img/magnifying-glass.png">
        </button>
        <button @click="$emit('cart-clicked')" class="trolly">
          <p>Tampilkan Menu</p>
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  computed: {
    cartSum () {
      return this.$store.state.cartSum
    }
  }
}
</script>

<style lang="scss" scoped>
nav {
  position: fixed;
  top: 0;
  width: 100%;
  background-color: #333333;
  box-shadow: 0 -4px 7px rgba(0, 0, 0, 0.733);
  font-size: 20px;
  font-weight: bold;
  padding: 6px 0;
  z-index: 2;
  transition: .3s;
  &.cart-on {
    width: 75vw;
  }
  div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    button {
      margin: 0 13px;
      padding: 10px;
      background-color: transparent;
      border: none;
      outline: none;
      cursor: pointer;
    }
    .burger {
      cursor: auto;
      img {
        height: 20px;
      }
    }
    .search {
      margin-right: 20px;
      img {
        height: 20px;
      }
    }
    .trolly.hidden {
      display: none;
    }
    .trolly {
      display: flex;
      align-items: center;
      margin-left: 0;
      padding-left: 0;
      img {
        height: 25px;
      }
    }
  }
}
</style>
