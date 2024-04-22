<template>
  <div class="container-fluid">
    <div class="text-center mb-5">
      <h3>KELOLA OBAT</h3>
    </div>
    <div>
      <form>
        <div class="row">
          <div class="col-lg-6">
            <div class="mb-3">
              <input type="number" class="form-control-lg rounded-2 border-dark" placeholder="Kode Obat" />
            </div>
            <div class="mb-3">
              <input type="text" class="form-control-lg rounded-2 border-dark" placeholder="Nama Obat" />
            </div>
            <div class="mb-3">
              <input type="date" class="form-control-lg rounded-2 border-dark" placeholder="Expired Date" style="width: 45vh;" />
            </div>
          </div>
          <div class="col-lg-3">
            <div class="mb-3">
              <input type="number" class="form-control-lg rounded-2 border-dark" placeholder="Jumlah" />
            </div>
            <input type="number" class="form-control-lg rounded-2 border-dark" placeholder="Harga" />
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
