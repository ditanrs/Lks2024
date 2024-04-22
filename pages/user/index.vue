<template>
  <div class="container-fluid">
    <div class="text-center">
      <h3>KELOLA USER</h3>
    </div>
    <div>
      <form>
        <div class="row">
          <div class="col-lg-6">
            <div class="mb-3">
              <input type="text" class="form-control form-control-lg rounded-2 border-dark" placeholder="Tipe user" />
            </div>
            <div class="mb-3">
              <input type="email" class="form-control form-control-lg rounded-2 border-dark" placeholder="Username" />
            </div>
          </div>
          <div class="col-lg-6">
            <div class="mb-3">
              <input type="text" class="form-control form-control-lg rounded-2 border-dark" placeholder="Nama" />
            </div>
            <input type="password" class="form-control form-control-lg rounded-2 border-dark" placeholder="Password" />
            <br />
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
            <td>Username</td>
            <td>Password</td>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td></td>
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
input {
  margin-left: 40%;
}
table {
  width: 70%;
  margin-left: 15%;
}
button {
  display: flex;
  justify-content: center;
  margin-left: 50%;
}
</style>
