<template>
  <div id="skills" class="container mx-auto mt-10 p-8">
    <h1 class="text-center text-4xl text-blue-700 font-bold">My skills</h1>
    <ul class="flex flex-wrap justify-center items-center mt-4">
      <p class="text-blue-700 text-center">
        I have a variety of skills that allow me to produce quality projects
        that meet code standards.
      </p>
    </ul>
    <div v-for="tab in tabs" :key="tab.id">
      <div
        v-if="tab.current"
        class="grid grid-flow-col justify-around grid-cols-3 grid-rows-4 gap-4 mt-12 mx-auto max-w-4xl"
      >
        <img
          v-for="skill in tab.skills"
          :key="skill"
          class="justify-self-center hover:shadow-lg transition duration-500"
          :alt="`${skill} banner`"
          :src="`/technologies/${skill}.svg`"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentTab: {},
      tabs: [
        {
          id: 'frameworks-and-librairies',
          name: 'Frameworks and librairies',
          current: true,
          skills: [
            'html',
            'css',
            'sass',
            'js',
            'laravel',
            'symfony',
            'node',
            'nuxt',
            'php',
            // 'wordpress',
            'composer',
            'tailwind',
            'bootstrap',
          ],
        },
      ],
    }
  },
  methods: {
    setCurrentTab(currentTabId) {
      this.tabs.map((tab) => {
        tab.current = tab.id === currentTabId
      })
    },
  },
}
</script>
