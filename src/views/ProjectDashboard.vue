<script setup lang="ts">
import { useI18n } from 'vue-i18n';

defineProps<{
  projectId: string;
  title?: string;
}>();
const { t } = useI18n();
</script>

<template>
  <main>
    <div class="grid">
      <h1>{{ t('projectDashboard.title', [projectId]) }}</h1>
    </div>
  </main>
</template>
