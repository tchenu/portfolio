<template>
  <span class="border rounded-full my-1 mr-2 py-1 px-2">
    <p class="inline">
      <span class="font-semibold">
        {{ name }}
      </span>
      <span v-if="years">
        {{ `· ${years}` }}
      </span>
    </p>
  </span>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: null,
    },
    years: {
      type: String,
      default: null,
    },
  },
}
</script>
