<template>
  <div class="container-fluid">
    <div class="text-center mt-5">
      <h3>Kelola Laporan</h3>
    </div>
    <h5>Laporan Penjualan</h5>

    <div class="row g-3 justify-content-center">
      <div class="col-auto">
        <label class="col-form-label">Dari tanggal</label>
      </div>
      <div class="col-auto">
        <input type="date" class="form-control" aria-describedby="passwordHelpInline" />
      </div>
      <div class="col-auto">
        <label class="col-form-label">Sampai tanggal</label>
      </div>
      <div class="col-auto">
        <input type="date" class="form-control" aria-describedby="passwordHelpInline" />
      </div>
      <button type="button" class="btn btn-outline-dark rounded-1">Apply</button>
    </div>

    <table class="table">
      <thead class="table-dark">
        <tr>
          <td>No</td>
          <td>Tanggal Transaksi</td>
          <td>Total bayar</td>
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
button {
  width: 5%;
  margin-left: 10px;
  background-color: #d3d1d1;
}
table {
  width: 70%;
  margin-left: 15%;
  margin-top: 5%;
}
h5{
    margin-left: 24%;
}
</style>
