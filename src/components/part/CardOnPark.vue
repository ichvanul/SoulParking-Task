<template>
  <div class="outline">
    <h3>List Petugas Parkir</h3>
    <div class="header">
      <div class="card-card">
        <div class="card-photo">
          <img src="../../assets/img/guys1.jpg">
        </div>
        <div class="card-data">
          <p class="name">Unggul</p>
          <div class="card-number">
            <i class="fas fa-mobile-alt"></i>
            <p>+6287776364745</p>
          </div>
          <div class="card-status">
            <i class="fas fa-check-circle"></i>
            <p>Aktif</p>
          </div>
        </div>
      </div>
    </div>

    <div class="header">
      <div class="card-card">
        <div class="card-photo">
          <img src="../../assets/img/guys2.jpg">
        </div>
        <div class="card-data">
          <p class="name">Hudya</p>
          <div class="card-number">
            <i class="fas fa-mobile-alt"></i>
            <p>+6287776364745</p>
          </div>
          <div class="card-status">
            <i class="fas fa-check-circle"></i>
            <p>Aktif</p>
          </div>
        </div>
      </div>
    </div>

    <div class="header">
      <div class="card-card">
        <div class="card-photo">
          <img src="../../assets/img/guys3.jpg">
        </div>
        <div class="card-data">
          <p class="name">Esa Kencana</p>
          <div class="card-number">
            <i class="fas fa-mobile-alt"></i>
            <p>+6287776364745</p>
          </div>
          <div class="card-status">
            <i class="fas fa-check-circle"></i>
            <p>Aktif</p>
          </div>
        </div>
      </div>
    </div>

    <div class="header">
      <div class="card-card">
        <div class="card-photo">
          <img src="../../assets/img/guys4.jpg">
        </div>
        <div class="card-data">
          <p class="name">Kusma Keling</p>
          <div class="card-number">
            <i class="fas fa-mobile-alt"></i>
            <p>+6287776364745</p>
          </div>
          <div class="card-status">
            <i class="fas fa-check-circle"></i>
            <p>Aktif</p>
          </div>
        </div>
      </div>
    </div>

    <div class="header">
      <div class="card-card">
        <div class="card-photo">
          <img src="../../assets/img/guys5.jpg">
        </div>
        <div class="card-data">
          <p class="name">Dhimas Sujipto</p>
          <div class="card-number">
            <i class="fas fa-mobile-alt"></i>
            <p>+6287776364745</p>
          </div>
          <div class="card-status">
            <i class="fas fa-check-circle"></i>
            <p>Aktif</p>
          </div>
        </div>
      </div>
    </div>

    <div class="header">
      <div class="card-card">
        <div class="card-photo">
          <img src="../../assets/img/guys6.jpg">
        </div>
        <div class="card-data">
          <p class="name">Sumatdja Alibaba</p>
          <div class="card-number">
            <i class="fas fa-mobile-alt"></i>
            <p>+6287776364745</p>
          </div>
          <div class="card-status">
            <i class="fas fa-check-circle"></i>
            <p>Aktif</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardOnPark'
}
</script>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
}

.outline {
  padding: 20px;
  background-color: white;
  border-radius: 10px;
  height: 990px;
  -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  h3 {
    font-size: 20px;
    font-weight: bolder;
    text-align: left;
    margin-bottom: 10px;
  }
}

.header {
  display: flex;
  flex-direction: column;
  border-radius: 2px;
  background-color: white;
  box-sizing: border-box;
  width: 390px;
  margin-bottom: 20px;
  -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  .card-card {
    display: flex;
    .name {
      font-weight: 600;
    }
    .card-photo {
      padding: 20px 0px 20px 20px;
      img {
      border-radius: 50%;
      width: 100px;
      height: 100px;
      object-fit: cover;
      }
    }
    .card-data {
      padding: 20px 100px 20px 20px;
      text-align: left;
      p {
        margin-bottom: 22px;
      }
      .card-number {
        display: flex;
        p {
          margin: 0 0 22px 10px;
        }
        i {
          font-size: 18px;
          color: orange;
        }
      }
      .card-status {
        display: flex;
        p {
          margin: 0 0 0 5px;
        }
        i {
          font-size: 18px;
          color: green;
        }
      }
    }
  }
}
</style>
