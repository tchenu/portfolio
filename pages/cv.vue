<template>
  <div>
    <Header class="print:hidden" />
    <div class="container mx-auto mt-0 md:mt-24">
      <div class="print:hidden">
        <h1 class="text-center text-4xl text-blue-700 font-bold">
          Curriculum vitæ
        </h1>
        <div class="text-center my-5">
          <WindowToPdf />
        </div>
      </div>
      <div
        id="cv"
        class="mt-4 mb-4 print:mt-0 shadow rounded print:shadow-none"
      >
        <CvMe />
        <CvResume />
        <CvSkills />
        <CvExperiences />
        <CvFormations />
        <CvLanguages />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head: {
    title: 'CV de Thibeault Chenu',
  },
}
</script>

<style>
@media print {
  @page {
    margin: 0;
  }

  #drift-widget-container {
    display: none;
  }
}

.experience:last-child,
.formation:last-child {
  border: none;
}
</style>
