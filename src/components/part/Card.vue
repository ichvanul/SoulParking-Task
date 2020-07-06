<template>
  <div class="card-header">
    <div class="card">
      <div class="content-header">
        <div class="title-header">
          <div class="title">
            <p>KEDATANGAN</p>
          </div>
          <div class="value">
            <p class="first">2.500</p>
          </div>
        </div>
        <div class="img-wrap">
          <i class="fas fa-sign-in-alt"></i>
        </div>
      </div>
      <div class="text-wrap">
        <p class="title-wrap"><span>+30%</span> dari minggu lalu</p>
      </div>
    </div>

    <div class="card">
      <div class="content-header">
        <div class="title-header">
          <div class="title">
            <p>PJP</p>
          </div>
          <div class="value">
            <p class="second">2.000</p>
          </div>
        </div>
        <div class="img-wrap">
          <i class="fas fa-redo-alt"></i>
        </div>
      </div>
      <div class="text-wrap">
        <p class="title-wrap"><span>+30%</span> dari minggu lalu</p>
      </div>
    </div>

    <div class="card">
      <div class="content-header">
        <div class="title-header">
          <div class="title">
            <p>PJP BARU</p>
          </div>
          <div class="value">
            <p class="third">500</p>
          </div>
        </div>
        <div class="img-wrap">
          <i class="fas fa-user-plus"></i>
        </div>
      </div>
      <div class="text-wrap">
        <p class="title-wrap"><span>+30%</span> dari minggu lalu</p>
      </div>
    </div>

    <div class="card">
      <div class="content-header">
        <div class="title-header">
          <div class="title">
            <p>KELUAR</p>
          </div>
          <div class="value">
            <p class="fourth">1.500</p>
          </div>
        </div>
        <div class="img-wrap">
          <i class="fas fa-sign-out-alt"></i>
        </div>
      </div>
      <div class="text-wrap">
        <p class="title-wrap"><span>+30%</span> dari minggu lalu</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card'
}
</script>

<style lang="scss" scoped>
.card-header {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.card {
  width: 270px;
  text-align: left;
  border-radius: 10px;
  background-color: white;
  overflow: hidden;
  margin: 0 25px;
  -webkit-box-shadow: 0px 0px 20px 0px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 0px 20px 0px rgba(0,0,0,0.75);
  box-shadow: 0px 0px 20px 0px rgba(0,0,0,0.75);
  .content-header {
    display: flex;
    .title-header {
      flex-direction: column;
      p {
        text-align: left;
        margin-top: 30px;
        margin-left: 10px;
        width: 110px;
      }
      .title {
        color: black;
        letter-spacing: 1px;
        font-weight: 600;
      }
      .value {
        font-size: 28px;
        font-weight: 600;
      }
      .first {
        color: #00e699;
      }
      .second {
        color: #9900e6;
      }
      .third {
        color: #005ce6;
      }
      .fourth {
        color: #e60000;
      }
    }
  }
  .img-wrap {
    width: 100%;
    height: 140px;
    overflow: hidden;
    text-align: center;
    i {
      font-size: 100px;
      margin-top: 20px;
    }
    .fa-sign-in-alt {
      color: #b3ffe6;
    }
    .fa-redo-alt {
      color: #e6b3ff;
    }
    .fa-user-plus {
      color: #b3d1ff;
    }
    .fa-sign-out-alt {
      color: #ffb3b3;
    }
  }
  .text-wrap {
    background-color: #ffd9b3;
    padding: 0px 0;
    height: 40px;
    .title-wrap {
      margin-left: 10px;
      padding-top: 10px;
      color: green;
      span {
        font-weight: bolder;
      }
    }
    .price {
      font-weight: bold;
      margin: 4px 0 8px;
    }
  }
  transition: .1s;
  &:hover {
    box-shadow: 0 5px 20px -10px rgba(0, 0, 0, 0.37);
    cursor: pointer;
  }
  &:active {
    transform: scale(0.97);
  }
}
</style>
