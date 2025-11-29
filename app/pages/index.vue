<template>
  <div>
    <fieldset
      style="margin-top: 30px; background-color: #c0c0c0"
      class="cv-fieldset"
    >
      <legend>My CV</legend>

      <PdfComponent />
    </fieldset>
  </div>
</template>
<script setup lang="ts"></script>
<style scoped>
@media screen and (max-width: 600px) {
  fieldset {
    max-width: 200px !important;
  }
}
</style>
