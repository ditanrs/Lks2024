<template>
  <nav class="navbar bg-light">
    <div class="container-fluid">
      <div class="col-lg-1">
        <img src="assets/img/logo.png" alt="logo" class="logo" />
      </div>
      <div class="col me-5">
        <h6>APOTEK XYZ</h6>
        <p>KASIR</p>
      </div>

      <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="offcanvas offcanvas-end bg-dark" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
        <div class="row justify-content-center">
          <div class="col-md offset-md-2">
            <div class="offcanvas-header">
              <img src="assets/img/kasir.png" alt="kasir" />
            </div>
            <div class="d-grid gap-2">
              <div class="btn1">
                <NuxtLink to="/transaksi" class="btn btn-light border-dark">Transaksi</NuxtLink>
              </div>
              <div class="btn1">
                <NuxtLink to="/transaksi/riwayat" class="btn btn-light border-dark">Riwayat</NuxtLink>
              </div>
              <button class="btn btn-danger mt-3" type="button">Logout</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.logo {
  width: 50px;
}

img {
  width: 50%;
}
.bg-light {
  background-color: #87bc9c !important;
}
.bg-dark {
  background-color: #b0ccbb !important;
}
.d-grid {
  width: 100%;
}
.btn {
  width: 70%;
}
</style>
