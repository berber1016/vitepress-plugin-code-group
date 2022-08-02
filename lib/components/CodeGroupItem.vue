<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'CodeGroupItem',
})
</script>

<script setup lang="ts">
defineProps({
  title: {
    type: String,
    required: true,
  },
  active: {
    type: Boolean,
    required: false,
    default: false,
  },
})
</script>

<style>
.code-group-item {
  display: none;
}

.code-group-item__active {
  display: block;
}

.code-group-item > pre {
  background-color: orange;
}
</style>

<template>
  <div
    class="code-group-item"
    :class="{ 'code-group-item__active': active }"
    :aria-selected="active"
  >
    <slot />
  </div>
</template>
