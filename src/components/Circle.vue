<template>
  <circle
    :cx="x"
    :cy="y"
    :r="r"
    @mousedown="$emit('start-drag-node', id)"
    @mouseup="$emit('end-drag-node')"
  />
</template>

<script lang="ts">
export default {
  name: 'Circle',
  props: {
    id: { type: Number, default: 0 },
    x: { type: Number, default: 0 },
    y: { type: Number, default: 0 },
    r: { type: Number, default: 0 },
  },
}
</script>
