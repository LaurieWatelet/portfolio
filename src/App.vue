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

  </div>
</template>

<script setup>
import PrimaryButton from './PrimaryButton.vue';
import Nav from './components/Nav.vue';
import Footer from './components/Footer.vue';
import Layout from './components/Layout.vue';
import NavLink from './NavLink.vue';
</script>

<style>
#app {
  height: 100vh;
}
</style>
