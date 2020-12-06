<template>
  <header class="mb-4" id="el_header">
    <div>
      <nav class="navbar navbar-dark bg-dark navbar-expand-sm">
          <a class="navbar-brand" href="#">
          <img src="../assets/logo.png" width="30" height="30" class="d-inline-block align-top" alt="logo" />
          Equipo #179
        </a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarToggler" aria-controls="navbarToggler" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
        <div class="collapse navbar-collapse justify-content-end" id="navbarToggler">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#el_header">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#services">Servicios</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#news">Noticias</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#team">Equipo</a>
          </li>
        </ul>
        </div>
      </nav>
    </div>
    <div class="container-imagen">
      <img class="img-fluid" style="width: 100%; height: 300px;" src="../../public/img/bg.png" alt="">
    </div>
  </header>
</template>

<script>
export default {
  name: "CabeceraPrincipal",
};
</script>