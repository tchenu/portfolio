<template>
  <div class="p-5 border-b border-grey-100">
    <h3
      class="text-blue-400 font-semibold text-sm uppercase mb-5 tracking-widest"
    >
      Compétences
    </h3>
    <h3
      class="text-blue-500 font-semibold text-md uppercase mb-2 tracking-widest"
    >
      Rôles
    </h3>
    <div class="flex flex-wrap mb-5">
      <Tag
        v-for="role in roles"
        :key="role.name"
        :name="role.name"
        :years="role.years"
      />
    </div>
    <h3
      class="text-blue-500 font-semibold text-md uppercase mb-2 tracking-widest"
    >
      Skills
    </h3>
    <div class="flex flex-wrap mb-5">
      <Tag
        v-for="skill in skills"
        :key="skill.name"
        :name="skill.name"
        :years="skill.years"
      />
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      roles: [
        {
          name: 'Développement back-end',
          years: '4 ans et +',
        },
        {
          name: 'Développement front-end',
          years: '4 ans et +',
        },
      ],
      skills: [
        {
          name: 'PHP ⭐️',
          years: '4 ans et +',
        },
        {
          name: 'HTML5',
          years: null,
        },
        {
          name: 'CSS3',
          years: null,
        },
        {
          name: 'JavaScript',
          years: null,
        },
        {
          name: 'jQuery',
          years: null,
        },
        {
          name: 'SQL',
          years: null,
        },
        {
          name: 'SASS',
          years: null,
        },
        {
          name: 'Laravel ⭐️',
          years: '4 ans et +',
        },
        {
          name: 'Symfony ⭐️',
          years: null,
        },
        {
          name: 'Bootstrap',
          years: null,
        },
        {
          name: 'Vue.js ⭐️',
          years: null,
        },
        {
          name: 'Nuxt.js',
          years: null,
        },
        {
          name: 'MySQL',
          years: null,
        },
        {
          name: 'API REST ⭐️',
          years: null,
        },
        {
          name: 'Wordpress',
          years: null,
        },
        {
          name: 'Node.js',
          years: null,
        },
        {
          name: 'Pentest ⭐️',
          years: null,
        },
        {
          name: 'Git',
          years: null,
        },
        {
          name: 'Docker',
          years: null,
        },
      ],
    }
  },
}
</script>
