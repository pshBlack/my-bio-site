<template>
  <VuePDF
    :pdf="pdf"
    style="display: flex; justify-content: center; margin: 5px 0px"
    fit-parent
    text-layer
    annotation-layer
    @annotation="onAnnotation"
  />
</template>
<script setup lang="ts">
import { VuePDF, usePDF } from "@tato30/vue-pdf";
import "@tato30/vue-pdf/style.css";
const { pdf } = usePDF("/Pavlo-Vysochynskyi-CV-ENG.pdf");

const onAnnotation = (value: any) => {
  if (value.type == "link") {
    window.open(value.data.url, "_blank");
  }
};
</script>
<style scoped></style>
