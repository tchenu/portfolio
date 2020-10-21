<template>
  <button
    class="px-10 py-3 text-white text-center bg-blue-600 rounded-md font-semibold align-middle"
    @click="print()"
  >
    {{ label }}
  </button>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: 'Download as PDF',
    },
  },
  methods: {
    print: () => {
      window.print()
    },
  },
}
</script>
