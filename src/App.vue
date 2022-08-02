<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import { CodeGroup,CodeGroupItem } from '../dist/codeGroup';

</script>

<template>
  <div>
    这是demo
  </div>
  <CodeGroup>
  <CodeGroupItem title="YARN" active>
    yarn
  </CodeGroupItem>
  <CodeGroupItem title="NPM">
    npm
  </CodeGroupItem>
</CodeGroup>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
