<template>
  <div class="container border-b border-grey-100 pb-3 my-5 experience">
    <div class="flex justify-between">
      <div class="flex flex-col justify-between text-left">
        <h3
          class="text-blue-500 font-semibold text-sm uppercase mb-3 tracking-widest"
        >
          {{ context }}
        </h3>
        <h4 class="text-2xl font-semibold">{{ client }}</h4>
      </div>
      <div class="flex flex-col justify-between text-right lowercase">
        <p>{{ fromFormatted }} - {{ toFormatted }}</p>
        <p v-if="!currently" class="text-blue-300 italic">
          {{ duration }}
        </p>
      </div>
    </div>
    <div class="flex flex-wrap my-3">
      <Tag v-for="tag in tags" :key="tag.name" :name="tag.name" />
    </div>
    <!-- eslint-disable-next-line vue/no-v-html -->
    <p class="text-gray-600" v-html="description"></p>
  </div>
</template>

<script>
import dayjs from 'dayjs'

const duration = require('dayjs/plugin/duration')
const relativeTime = require('dayjs/plugin/relativeTime')
const isToday = require('dayjs/plugin/isToday')

require('dayjs/locale/fr')

dayjs.extend(duration)
dayjs.extend(relativeTime)
dayjs.extend(isToday)

export default {
  props: {
    context: {
      type: String,
      default: null,
    },
    client: {
      type: String,
      default: null,
    },
    from: {
      type: Date,
      default: null,
    },
    to: {
      type: Date,
      default: null,
    },
    description: {
      type: String,
      default: null,
    },
    tags: {
      type: Array,
      default: null,
    },
  },
  data: () => {
    return {
      duration: null,
      currently: false,
      fromFormatted: null,
      toFormatted: null,
    }
  },
  mounted() {
    const from = dayjs(this.from).locale('fr')
    const to = dayjs(this.to).locale('fr')

    this.currently = to.isToday()
    this.fromFormatted = from.format('MMMM YYYY')
    this.toFormatted = to.isToday() ? 'En cours' : to.format('MMMM YYYY')
    this.duration = dayjs.duration(from.diff(to)).locale('fr').humanize()
  },
}
</script>
