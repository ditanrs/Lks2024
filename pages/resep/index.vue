<template>
  <div class="container-fluid">
    <div class="text-center mb-5">
      <h3>KELOLA RESEP</h3>
    </div>
    <div>
      <form>
        <div class="row">
          <div class="col-lg-4 ms-5">
            <div class="mb-3">
              <input type="number" class=" form-control-lg rounded-2 border-dark" placeholder="No Resep" />
            </div>
            <div class="mb-3">
              <input type="text" class=" form-control-lg rounded-2 border-dark" placeholder="Nama Pasien" />
            </div>
            <div class="mb-3">
              <input type="text" class=" form-control-lg rounded-2 border-dark" placeholder="Nama Obat" />
            </div>
          </div>
          <div class="col-lg-2">
            <div class="mb-3">
              <input type="date" class=" form-control-lg rounded-2 border-dark" style="width: 45vh;" />
            </div>
            <div class="mb-3">
              <input type="text" class=" form-control-lg rounded-2 border-dark" placeholder="Nama Dokter" />
            </div>
            <div class="mb-3">
              <input type="number" class=" form-control-lg rounded-2 border-dark" placeholder="Quantity" />
            </div>
          </div>
        </div>

        <button type="submit" class="btn btn-success text-white bg-success rounded-2 px-4 text-center mb-5 mt-3">KIRIM</button>
      </form>
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
  margin-left: 70%;
}
table {
  width: 70%;
  margin-left: 15%;
}
button {
  display: flex;
  justify-content: center;
  margin-left: 45%;
}
.col-auto {
  margin-left: 15%;
}
label {
  margin-left: 5%;
}
</style>
