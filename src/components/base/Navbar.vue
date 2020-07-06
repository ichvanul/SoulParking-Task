<template>
  <nav>
    <div>
      <div>
        <button @click="$emit('cart-clicked')" class="trolly">
          <p>Tampilkan Menu</p>
        </button>
      </div>
      <select name="city" id="city">
        <option value="DKI Jakarta">DKI Jakarta</option>
        <option value="Bandung">Bandung</option>
        <option value="Semarang">Semarang</option>
        <option value="Makassar">Makassar</option>
      </select>
      <div class="account">
        <div><img src="../../assets/img/guys6.jpg"></div>
        <div class="content">
          <p class="name">Husein Damar</p>
          <p class="status">Super Admin</p>
        </div>
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
    justify-content: flex-start;
    align-items: center;
    button {
      margin: 0 13px;
      padding: 10px;
      background-color: transparent;
      border: none;
      outline: none;
      cursor: pointer;
    }
    .trolly.hidden {
      display: none;
    }
    .trolly {
      display: flex;
      align-items: center;
      margin-right: 0;
      padding-right: 0;
      img {
        height: 25px;
      }
      p {
        color: white;
        font-size: 14px;
        line-height: 20px;
        font-weight: bold;
        width: 200px;
      }
    }
    select {
      margin: 7px 0 7px 650px;
      padding: 3px 50px 3px 0;
      border-radius: 5px;
    }
    img {
      border-radius: 50%;
      width: 40px;
      height: 40px;
      object-fit: cover;
    }
    .content {
      display: flex;
      flex-direction: column;
      color: white;
      font-size: 12px;
      .status {
        font-weight: 500;
        p {
          text-align: left;
        }
      }
      .name {
        margin-left: 11px;
        margin-bottom: 3px;
      }
    }
  }
}

.account {
  margin-left: 60px;
}
</style>
