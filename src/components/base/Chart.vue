<template>
  <div class="header">
    <div class="left">
      <div class="chart-pie">
        <h3>TOTAL PEMASUKAN</h3>
        <bar-chart class="pie"
        :data="[['Januari', 10],['Februari', 25],['Maret', 55],['April', 10],['Mei', 10],['Juni', 10],['Juli', 10],['Agustus', 10],['September', 10],['Oktober', 10],['November', 10],['Desember', 10]]">
        </bar-chart>
      </div>
        <div class="chart-pie pie2">
        <h3>MEMBERSHIP</h3>
        <bar-chart class="pie"
        :data="[['Januari', 10],['Februari', 25],['Maret', 55],['April', 10],['Mei', 10],['Juni', 10],['Juli', 10],['Agustus', 10],['September', 10],['Oktober', 10],['November', 10],['Desember', 10]]">
        </bar-chart>
      </div>
    </div>
    <div class="right">
      <div class="chart-pie">
        <h3>METODE PEMBAYARAN</h3>
        <pie-chart class="pie"
        :data="[['CASH', 800],['GO-PAY', 150],['MEMBERSHIP', 50]]">
        </pie-chart>
      </div>
        <div class="chart-pie pie3">
        <h3>TRAFIK SITUS</h3>
        <pie-chart class="pie" :data="[['Organic Search', 10],['Direct', 25],['Social', 55],['Other', 10]]"></pie-chart>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Chart'
}
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  flex-direction: column;
  .left {
    display: flex;
    flex-direction: row;
    .chart-pie {
      border: 2px solid white ;
      border-radius: 5px;
      background-color: white;
      padding: 10px 140px;
      margin: 25px;
      -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      h3 {
        text-align: left;
        font-weight: bold;
      }
    }
  }
  .right {
    display: flex;
    flex-direction: row;
    .chart-pie {
      border: 2px solid white ;
      border-radius: 5px;
      background-color: white;
      padding: 10px 140px;
      margin: 25px;
      -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      h3 {
        text-align: left;
        font-weight: bold;
        font-size: 16px;
      }
    }
  }
}
</style>
