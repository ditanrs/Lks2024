<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="text-center mb-5">
          <h3>KELOLA USER</h3>
        </div>
        <form>
          <div class="mb-3">
            <div class="row">
              <div class="col-lg-3">
                <select class="form-control form-control-lg form-select rounded-2 border-dark me-5">
                  <option>Tipe User</option>
                  <option>Admin</option>
                  <option>Apoteker</option>
                  <option>Kasir</option>
                </select>
              </div>
              <div class="col-lg-3">
                <input type="text" class="form-control form-control-lg rounded-2 border-dark me-5 mb-4" placeholder="Username" />
              </div>
            </div>

            <div class="row">
              <div class="col-lg-3">
                <input type="email" class="form-control form-control-lg rounded-2 border-dark me-5" placeholder="Email" />
              </div>

              <div class="col-lg-3">
                <input type="password" class="form-control form-control-lg rounded-2 border-dark" placeholder="Password" />
              </div>
            </div>
          </div>
          <button type="submit" class="btn btn-success text-white bg-success rounded-2 px-4 text-center mb-5">Tambah</button>
        </form>
      </div>
    </div>
  </div>

  <div>
    <table class="table">
      <thead class="table-dark">
        <tr>
          <td>Tipe User</td>
          <td>Username</td>
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
</template>

<style scoped>
.container-fluid {
  margin-top: 2%;
}
.bg-success {
  background-color: #019901 !important;
}

table {
  width: 70%;
  margin-left: 15%;
}
button {
  margin-left: 45%;
}
</style>
