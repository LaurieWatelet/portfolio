<template>
  <div>
    <!-- Titre de la page -->
    <slot name="title"></slot>

    <!-- Contenu principal de la page -->
    <slot name="content"></slot>
  </div>
</template>

<script>
export default {
  name: 'Layout'
};
</script>