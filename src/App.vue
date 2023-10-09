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

  </div>
</template>

<script setup>
import PrimaryButton from './PrimaryButton.vue';
import Nav from './components/Nav.vue';
import Footer from './components/Footer.vue';
</script>

<style>
#app {
  height: 100vh;
}
</style>
