<template>
  <div class="d-flex flex-column h-100">
    <header>
      <!-- Utilisation du composant Nav -->
      <Nav /> 
      <!-- Remplacez le code du navbar par cette balise -->
    </header>

    <!-- Begin page content -->
    <main class="flex-shrink-0 py-5">
      <div class="container">


      </div>
    </main>

    <footer class="footer mt-auto py-3 bg-body-tertiary">

    </footer>
    <!-- Utilisation du composant Footer -->

    <PrimaryButton>
      Cliquez ici <!-- slot -->
    </PrimaryButton>

   <Layout>
    <template v-slot:title>
      <h1 class="mt-5">Sticky footer with fixed navbar</h1>
    </template>

    <template v-slot:content>
      <p class="lead">
        Pin a footer to the bottom of the viewport in desktop browsers with this
        custom HTML and CSS. A fixed navbar has been added with
        <code class="small">padding-top: 60px;</code> on the
        <code class="small">main &gt; .container</code>.
      </p>
      <p>
        Back to
        <a href="/docs/5.3/examples/sticky-footer/"
          >the default sticky footer</a
        >
        minus the navbar.
      </p>
    </template>
  </Layout>

  <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Fixed navbar</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarCollapse"
        aria-controls="navbarCollapse"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarCollapse">
        <ul class="navbar-nav me-auto mb-2 mb-md-0">
          <NavLink url="#" text="Home" :isActive="true" />
          <NavLink url="#" text="Link" />
          <NavLink text="Disabled" :isDisabled="true" />
        </ul>
        <form class="d-flex" role="search">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>

  <Layout>
    <RouterView />
  </Layout>

  </div>
</template>

<script setup>
import Nav from './components/Nav.vue';
import Footer from './components/Footer.vue';
import Layout from './components/Layout.vue';
import { RouterView } from 'vue-router';
import NavLink from './components/NavLink.vue';
</script>

<style>
#app {
  height: 100vh;
}
</style>
