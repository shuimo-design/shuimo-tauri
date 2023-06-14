<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup


import { ref } from 'vue';
import DragHeader from './components/DragHeader.vue';

const info = ref('123312');
</script>

<template>
  <m-border>
    <m-rice-paper>
      <DragHeader/>
      <div class="container">
        <span>{{info}}</span>
        <div>
          <m-input v-model="info"></m-input>
          <m-button>确定</m-button>
        </div>
      </div>
    </m-rice-paper>
  </m-border>
</template>

<style scoped>
.logo.vite:hover {
  filter: drop-shadow(0 0 2em #747bff);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #249b73);
}
</style>
