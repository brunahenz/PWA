<script setup>
  import { useMonitor } from '@/composables/monitor';

  const { menu } = useMonitor();
</script>

<template>
  <div>
    <component :is="menu" />
    <main>
      <router-view />
    </main>
    <footer>
      <p>Copyright &copy; 2024</p>
      <component :is="menu" />
    </footer>
  </div>
</template>
