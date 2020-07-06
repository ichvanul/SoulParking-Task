<template>
  <div class="cart">
    <div class="cart-header">
      <div @click="$emit('cart-clicked')" >
        <button class="trolly">
          <img src="http://soulparking.co.id/images/logo.png">
        </button>
      </div>
    </div>
    <div class="sidebar">
     <ul>
      <router-link to="/">
        <li><a href="#"><i class="fas fa-th-large"> Dashboard </i></a></li>
      </router-link>
        <li>
          <a href="#"><i class="fas fa-book"> Pelaporan
            <span class="fas fa-caret-down"></span>
          </i></a>
          <ul>
            <li><a href="#">Laporan Trafik</a></li>
            <li><a href="#">Laporan Pendapatan</a></li>
            <li><a href="#">Pengaduan</a></li>
            <li><a href="#">Laporan Member</a></li>
            <li><a href="#">Laporan Gaskir</a></li>
            <li><a href="#">Laporan Aplikasi</a></li>
          </ul>
        </li>
        <li>
          <a href="#"><i class="fas fa-cog"> Pengaturan Lokasi
            <span class="fas fa-caret-down"></span>
          </i></a>
          <ul>
            <li><a href="#">Info Lokir</a></li>
            <li><a href="#">Tarif</a></li>
            <router-link to="/gaskir">
              <li><a class="gaskir">Gaskir</a></li>
            </router-link>
            <li><a href="#">Shift</a></li>
            <li><a href="#">Produk</a></li>
            <li><a href="#">Pemutihan Kendaraan</a></li>
            <li><a href="#">Aktivasi Member</a></li>
          </ul>
        </li>
        <li>
          <a href="#"><i class="fas fa-user"> Sistem Admin
            <span class="fas fa-caret-down"></span>
          </i></a>
          <ul>
            <li><a href="#">Lokir</a></li>
            <li><a href="#">Pengguna</a></li>
            <li><a href="#">Hardware</a></li>
          </ul>
        </li>
        <li><a href="#"><i class="fas fa-user-circle"> Sistem Admin </i></a></li>
        <li><a href="#"><i class="fas fa-sign-out-alt"> Keluar </i></a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cart'
}
</script>

<style lang="scss" scoped>
.cart {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 3;
  background-color: white;
  width: 0vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  box-shadow: 4px 0 7px rgba(0, 0, 0, 0.733);
  overflow: hidden;
  transition: .3s;
  &.active {
    width: 25vw;
  }
}
.cart-header, .wrap-body {
  width: 100%;
}
.cart-header {
  padding: 12.5px 0;
  box-shadow: 0 -4px 7px rgba(0, 0, 0, 0.733);
  div {
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
  }
  .trolly {
    margin: 0 5px 0 0;
    background-color: transparent;
    border: none;
    cursor: pointer;
    outline: none;
    img {
      height: 25px;
    }
  }
}

.sidebar {
  overflow-y: scroll;
  &::-webkit-scrollbar {
    width: 10px;
  }
  &::-webkit-scrollbar-thumb {
    background-color: #dbdbdb;
    border-radius: 10px;
  }
  &::-webkit-scrollbar-track {
    background-color: transparent;
    border-radius: 10px;
  }
}

ul {
    background: white;
    list-style: none;
    li {
      line-height: 40px;
      a {
        position: relative;
        text-align: left;
        color: black;
        text-decoration: none;
        font-size: 16px;
        padding-left: 30px;
        font-weight: 500;
        display: block;
        border-left: 3px solid transparent;
        span {
          position: absolute;
          top: 50%;
          right: 25px;
          transform: translateY(-50%);
          font-size: 20px;
          transition: transform 0.4s;
        }
        .gaskir {
          padding-left: 16px;
        }
      }
      a:hover {
        color: white;
        background: orange;
        border-left-color: orange;
        span {
          transform: translateY(-50%) rotate(-180deg);
        }
      }
    }
    ul {
      position: static;
      // display: none;
      li {
        line-height: 30px;
        border-bottom: none;
        a {
          font-size: 14px;
          color: black;
          padding-left: 50px;
          text-align: left;
        }
      }
    }
  }

  @media only screen and (max-width: 768px) {
  /* For mobile phones: */
  .cart {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 3;
  background-color: white;
  width: 0vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  box-shadow: 4px 0 7px rgba(0, 0, 0, 0.733);
  overflow: hidden;
  transition: .3s;
  &.active {
    width: 75vw;
  }
}
.cart-header, .wrap-body {
  width: 100%;
}
.cart-header {
  padding: 12.5px 0;
  box-shadow: 0 -4px 7px rgba(0, 0, 0, 0.733);
  div {
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
  }
  .trolly {
    margin: 0 5px 0 0;
    background-color: transparent;
    border: none;
    cursor: pointer;
    outline: none;
    img {
      height: 25px;
    }
  }
}

.sidebar {
  overflow-y: scroll;
  &::-webkit-scrollbar {
    width: 10px;
  }
  &::-webkit-scrollbar-thumb {
    background-color: #dbdbdb;
    border-radius: 10px;
  }
  &::-webkit-scrollbar-track {
    background-color: transparent;
    border-radius: 10px;
  }
}

ul {
    background: white;
    list-style: none;
    li {
      line-height: 40px;
      a {
        position: relative;
        text-align: left;
        color: black;
        text-decoration: none;
        font-size: 16px;
        padding-left: 30px;
        font-weight: 500;
        display: block;
        border-left: 3px solid transparent;
        span {
          position: absolute;
          top: 50%;
          right: 25px;
          transform: translateY(-50%);
          font-size: 20px;
          transition: transform 0.4s;
        }
        .gaskir {
          padding-left: 16px;
        }
      }
      a:hover {
        color: white;
        background: orange;
        border-left-color: orange;
        span {
          transform: translateY(-50%) rotate(-180deg);
        }
      }
    }
    ul {
      position: static;
      // display: none;
      li {
        line-height: 30px;
        border-bottom: none;
        a {
          font-size: 14px;
          color: black;
          padding-left: 50px;
          text-align: left;
        }
      }
    }
  }
  }
</style>
