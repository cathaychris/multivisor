<template lang="html">
  <div>
    <span v-if="process.gui_url">{{ process.name }} (<v-tooltip right><a :href="process.gui_url" target="_blank" slot="activator">{{ process.gui_name }}</a><span>{{ process.gui_desc }}</span></v-tooltip>)</span>
    <span v-else>{{ process.name }}</span>
  </div>
</template>

<script>
export default {
  name: 'ProcessCircus',
  props: ['process']
}
</script>
