<template>
  <div>
    <fieldset
      style="margin-top: 30px; margin-right: 2px; background-color: #c0c0c0"
    >
      <legend>My CV</legend>
      <div v-if="loading">
        <div class="progress-indicator segmented">
          <span
            class="progress-indicator-bar"
            :style="{ width: progress + '%' }"
          />
        </div>
      </div>

      <iframe
        src="/Pavlo-Vysochynskyi-CV-ENG.pdf"
        width="100%"
        height="700px"
        v-show="!loading"
        @load="loading = false"
      />
    </fieldset>
  </div>
</template>
<script setup lang="ts">
const loading = ref(true);
const progress = ref(0);

onBeforeMount(() => {
  const interval = setInterval(() => {
    if (progress.value < 100) {
      progress.value += 10;
    } else {
      clearInterval(interval);
      loading.value = false;
    }
  }, 50);
});
</script>
