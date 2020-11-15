<template>
  <div class="container border-b border-grey-100 pb-3 mt-5 formation">
    <div class="flex justify-between">
      <div class="flex flex-col justify-between text-left">
        <h3
          class="text-blue-500 font-semibold text-sm uppercase mb-3 tracking-widest"
        >
          {{ diploma }}
        </h3>
        <h4 class="text-2xl font-semibold">{{ school }}</h4>
      </div>
      <div class="flex flex-col justify-between text-right lowercase">
        <p>{{ fromFormatted }} - {{ toFormatted }}</p>
        <p v-if="!currently" class="text-blue-300 italic">
          {{ duration }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import dayjs from 'dayjs'

const duration = require('dayjs/plugin/duration')
const relativeTime = require('dayjs/plugin/relativeTime')
const isToday = require('dayjs/plugin/isToday')

dayjs.extend(duration)
dayjs.extend(relativeTime)
dayjs.extend(isToday)

export default {
  props: {
    diploma: {
      type: String,
      default: null,
    },
    school: {
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
    this.fromFormatted = from.format('YYYY')
    this.toFormatted = to.isToday() ? 'En cours' : to.format('YYYY')
  },
}
</script>
