<template>
  <div class="p-5 border-b border-grey-100">
    <h3
      class="text-blue-400 font-semibold text-sm uppercase mb-5 tracking-widest"
    >
      Formation
    </h3>
    <CvFormation
      v-for="(formation, index) in formations"
      :key="index"
      :diploma="formation.diploma"
      :school="formation.school"
      :from="formation.from"
      :to="formation.to"
    />
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      formations: [
        {
          school: 'ESGI',
          diploma: 'Mastère Ingénierie du Web en alternance',
          from: new Date(2020, 8),
          to: new Date(),
        },
        {
          school: 'ESGI',
          diploma: 'Bachelor Ingénierie du Web en alternance',
          from: new Date(2019, 8),
          to: new Date(2020, 8),
        },
        {
          school: 'Université Paris 13',
          diploma: 'DUT informatique en alternance',
          from: new Date(2017, 8),
          to: new Date(2019, 8),
        },
      ],
    }
  },
}
</script>
