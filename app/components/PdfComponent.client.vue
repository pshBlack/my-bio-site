<template>
  <VuePDF
    :pdf="pdf"
    style="display: flex; justify-content: center; margin: 5px 0px"
    :width="width"
  />
</template>
<script setup lang="ts">
import { VuePDF, usePDF } from "@tato30/vue-pdf";
import "@tato30/vue-pdf/style.css";
const { pdf } = usePDF("/Pavlo-Vysochynskyi-CV-ENG.pdf");
const width = computed(() => window.innerWidth / 2);
</script>
<style scoped></style>
