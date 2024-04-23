<template>
  <div class="container-fluid">
    <div class="row">
      <div class="text-center mb-5">
        <h3>KELOLA OBAT</h3>
      </div>
      <form>
        <div class="mb-3 container">
          <div class="row">
            <div class="col-lg-6 pt-2">
              <input type="number" class="form-control form-control-lg rounded-2 border-dark" placeholder="Kode Obat" />
            </div>
            <div class="col-lg-6 pt2">
              <input type="text" class="form-control form-control-lg rounded-2 border-dark" placeholder="Nama Obat" />
            </div>
          </div>

          <div class="row">
            <div class="col-lg-6 pt-2">
              <input type="date" class="form-control form-control-lg rounded-2 border-dark" placeholder="Expired Date" />
            </div>

            <div class="col-lg-6 pt-2">
              <input type="number" class="form-control form-control-lg rounded-2 border-dark" placeholder="Jumlah" />
            </div>
          </div>
          <div class="col-lg-6 pt-2">
            <input type="number" class="form-control form-control-lg rounded-2 border-dark" placeholder="Harga" />
          </div>
        </div>
        <div class="col-lg-12">
          <button type="submit" class="btn btn-success text-white bg-success rounded-2 px-4 text-center mb-5">Tambah</button>
        </div>
      </form>
    </div>
  </div>

  <div>
    <table class="table">
      <thead class="table-dark">
        <tr>
          <td>Kode Obat</td>
          <td>Nama Obat</td>
          <td>Expired Date</td>
          <td>Jumlah</td>
          <td>Harga</td>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td></td>
          <td></td>
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
