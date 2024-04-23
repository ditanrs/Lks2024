<template>
  <div class="container-fluid">
    <div class="row">
      <div class="text-center mb-5">
        <h3>KELOLA RESEP</h3>
      </div>
      <form>
        <div class="mb-3 container">
          <div class="row">
            <div class="col-lg-6 pt-2">
              <input type="number" class="form-control form-control-lg rounded-2 border-dark" placeholder="No Resep" />
            </div>
            <div class="col-lg-6 pt2">
              <input type="text" class="form-control form-control-lg rounded-2 border-dark" placeholder="Nama Pasien" />
            </div>
          </div>

          <div class="row">
            <div class="col-lg-6 pt-2">
              <input type="text" class="form-control form-control-lg rounded-2 border-dark" placeholder="Nama Obat" />
            </div>

            <div class="col-lg-6 pt-2">
              <input type="date" class="form-control form-control-lg rounded-2 border-dark" />
            </div>
          </div>

          <div class="row">
            <div class="col-lg-6 pt-2">
              <input type="text" class="form-control form-control-lg rounded-2 border-dark" placeholder="Nama Dokter" />
            </div>

            <div class="col-lg-6 pt-2">
              <input type="number" class="form-control form-control-lg rounded-2 border-dark" placeholder="Quantity" />
            </div>
          </div>
        </div>
        <div class="col-lg-12">
          <button type="submit" class="btn btn-success text-white bg-success rounded-2 px-4 text-center mb-5 mt-3">KIRIM</button>
        </div>
      </form>
    </div>
  </div>
</template>

<style scoped>
.container-fluid {
  margin-top: 2%;
}
.bg-success {
  background-color: #019901 !important;
}
button {
  margin-left: 45%;
}
</style>
