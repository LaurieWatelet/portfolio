<script setup></script>
<template>
  <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-primary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Portfolio</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarCollapse"
        aria-controls="navbarCollapse"
        aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarCollapse">
        <ul class="navbar-nav me-auto mb-2 mb-md-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Accueil</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Projets</a>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled" aria-disabled="true">À propos</a>
          </li>
        </ul>
        <form class="d-flex" role="search">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Recherche"
            aria-label="Search"
          />
          <button class="btn btn-outline-success" type="submit">Recherche</button>
        </form>
      </div>
    </div>
  </nav>
</template>
