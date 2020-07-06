<template>
  <div class="header">
    <form>
      <div class="form-content">
        <div class="input" >
          <label for="name" class="label">Nama Petugas Parkir</label>
          <input placeholder="Partejo Sukowon" type="text" class="input-form" id="name">
        </div>
        <div class="input" >
          <label for="code" class="label">NIK</label>
          <input placeholder="3208121111820001" type="number" class="input-form" id="code">
        </div>
        <div class="input" >
          <label for="number" class="label">No. Telepon</label>
          <input placeholder="081234275296" type="number" class="input-form" id="number">
        </div>
      </div>
      <div class="form-content">
        <div class="input" >
          <label for="username" class="label">Username</label>
          <input placeholder="Partejo203" type="text" class="input-form" id="username">
        </div>
        <div class="input" >
          <label for="password" class="label">Password</label>
          <input placeholder="Password" type="password" class="input-form" id="password">
        </div>
        <div class="input">
          <label for="check" class="label">Aktif</label>
          <input class="input-check" type="checkbox" id="check" value="option">
        </div>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'Form'
}
</script>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
}

.header {
  form {
    display: flex;
    width: 500px;
    .form-content {
      margin: 12px 12px;
      .input {
        display: flex;
        flex-direction: column;
        .label {
          text-align: left;
          font-weight: bold;
          font-size: 14px;
          margin: 10px 0;
          margin-top: 22px;
        }
        .input-form {
          width: 280px;
          border: 1px solid gainsboro;
          padding: 8px 5px;
          border-radius: 5px;
        }
        .input-check {
          justify-content: left;
          border: 1px solid gainsboro;
        }
      }
    }
  }
}
</style>
