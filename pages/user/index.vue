<template>
  <div class="container-fluid">
    <div class="text-center mb-5">
      <h3>KELOLA USER</h3>
    </div>
    <div>
      <form>
        <div class="row">
          <div class="in1">
            <div class="mb-3">
              <input type="text" class="form-control-lg rounded-2 border-dark mb-3 me-5" placeholder="Tipe user" />
              <input type="text" class="form-control-lg rounded-2 border-dark me-5" placeholder="Nama" />
            </div>
            <div class="mb-3">
              <input type="email" class="form-control-lg rounded-2 border-dark me-5" placeholder="Email" />
              <input type="password" class="form-control-lg rounded-2 border-dark" placeholder="Password" />
              <br />
            </div>
          </div>
        </div>
        <button type="submit" class="btn btn-success text-white bg-success rounded-2 px-4 text-center mb-5">Tambah</button>
      </form>
    </div>
    <div>
      <table class="table">
        <thead class="table-dark">
          <tr>
            <td>Tipe User</td>
            <td>Nama</td>
            <td>Email</td>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td></td>
            <td></td>
            <td></td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<style scoped>
.form-control {
  width: 25%;
}
.container-fluid {
  margin-top: 2%;
}
.bg-success {
  background-color: #019901 !important;
}
.in1 {
  margin-left: 25%;
}

table {
  width: 70%;
  margin-left: 15%;
}
button {
  margin-left: 45%;
}
</style>
