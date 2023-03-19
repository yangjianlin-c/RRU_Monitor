<script setup lang="ts">
import Dashboard from './components/Dashboard.vue'
</script>

<template>
  
  <Dashboard />


  <select id="serialPorts">
    <option value="">--Please choose a serial port--</option>
    <!-- use JavaScript to dynamically populate options -->
  </select>
  
</template>
