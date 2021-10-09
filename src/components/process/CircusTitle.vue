<template lang="html">
<div>
  <a v-if="process.gui_url" :href="process.gui_url" target="_blank">{{ process.name }}</a>
  <span v-else>{{ process.name }}</span>
  </div>
</template>

<script>
export default {
  name: 'ProcessCircus',
  props: ['process']
}
</script>
