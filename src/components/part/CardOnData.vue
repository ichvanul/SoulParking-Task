<template>
  <div class="header">
    <h3>Upload Dokumen Data Diri</h3>
    <div class="header-upload">
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
    <h3>Informasi Lokasi Parkir</h3>
    <Form class="form"/>
    <div class="button">
      <button class="cancel">BATAL</button>
      <button class="ok">SIMPAN</button>
    </div>
  </div>
</template>

<script>
import Form from '../base/Form'
export default {
  name: 'CardOnData',
  components: {
    Form
  }
}
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  flex-direction: column;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  margin-left: 40px;
  height: 990px;
  -webkit-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  box-shadow: 0px 10px 20px -13px rgba(0,0,0,0.75);
  h3 {
    text-align: left;
    font-weight: bold;
    font-size: 20px;
    margin: 0 20px;
  }
  .header-upload {
    display: flex;
    .upload-data {
      display: flex;
      flex-direction: column;
      align-items: center;
      border: 2px solid gainsboro;
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
          color: gainsboro;
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
  .form {
    margin: 0;
    padding: 0;
    border: 2px solid gainsboro;
    width: 636px;
    height: 300px;
    margin-left: 20px;
    margin-top: 20px;
    box-shadow: none;
  }
  .button {
    margin-top: 100px;
    display: flex;
    justify-content:flex-end;
    .cancel {
      border: 1px solid red;
      background-color: white;
      border-radius: 5px;
      color: red;
      font-weight: 600;
      padding: 10px 35px;
      margin-right: 40px;
      cursor: pointer;
      outline: none;
    }
    .ok {
      border: 1px solid orange;
      border-radius: 5px;
      background-color: orange;
      color: white;
      font-weight: 600;
      padding: 10px 35px;
      margin-right: 20px;
      cursor: pointer;
      outline: none;
    }
  }
}
</style>
