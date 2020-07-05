<template>
  <div class="header">
    <div class="upload-data">
      <div class="upload">
        <i class="fas fa-cloud-upload-alt"></i>
      </div>
      <button>UPLOAD KTP</button>
      <p>Ekstensi file yang diperbolehkan: <span>.JPG .JPEG .PNG</span></p>
    </div>
    <div class="upload-data">
      <div class="upload">
        <i class="fas fa-cloud-upload-alt"></i>
      </div>
      <button class="photo">UPLOAD FOTO DIRI</button>
      <p>Ekstensi file yang diperbolehkan: <span>.JPG .JPEG .PNG</span></p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardOnData'
}
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  margin-left: 40px;
  height: 950px;
  -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  .upload-data {
    display: flex;
    flex-direction: column;
    align-items: center;
    border: 2px solid whitesmoke;
    border-radius: 10px;
    height: 370px;
    margin: 20px;
    padding: 0 10px;
    .upload {
      margin-bottom: 10px;
      i {
        font-size: 100px;
        border: 1px solid white;
        border-radius: 5px;
        color: whitesmoke;
        margin: 20px 0;
        padding: 60px;
        -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
        -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
        box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
      }
    }
    button {
      background-color: orange;
      border-radius: 10px;
      outline: none;
      color: white;
      font-weight: bolder;
      width: 120px;
      border: none;
      cursor: pointer;
      padding: 10px;
      margin-bottom: 25px;
    }
    .photo {
      width: 150px;
    }
    p {
      font-size: 12px;
      span {
        font-weight: bold;
      }
    }
  }
}
</style>
