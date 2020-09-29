<template>
  <div id="skills" class="container mx-auto mt-10 p-8">
    <h1 class="text-center text-4xl text-blue-700 font-bold">My skills</h1>
    <ul class="flex flex-wrap justify-center items-center mt-8">
      <li
        class="mx-5 xs:p-0 p-3 bg-blue-200 text-blue-700 rounded transition duration-500 cursor-pointer font-medium"
      >
        Frameworks and librairies
      </li>
      <li
        class="mx-5 p-3 text-blue-700 hover:bg-blue-200 hover:font-medium rounded transition duration-500 cursor-pointer font-regular"
      >
        Langages
      </li>
      <li
        class="mx-5 p-3 text-blue-700 hover:bg-blue-200 hover:font-medium rounded transition duration-500 cursor-pointer font-regular"
      >
        Databases
      </li>
      <li
        class="mx-5 p-3 text-blue-700 hover:bg-blue-200 hover:font-medium rounded transition duration-500 cursor-pointer font-regular"
      >
        CMS
      </li>
      <li
        class="mx-5 p-3 text-blue-700 hover:bg-blue-200 hover:font-medium rounded transition duration-500 cursor-pointer"
      >
        <img src="~/assets/icons/next.svg" />
      </li>
    </ul>
    <div
      class="grid grid-flow-col justify-around grid-cols-3 grid-rows-3 gap-4 mt-16"
    >
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/laravel.svg" />
      </div>
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/php.svg" />
      </div>
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/sass.svg" />
      </div>

      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/laravel.svg" />
      </div>
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/php.svg" />
      </div>
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/vue.svg" />
      </div>
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/sass.svg" />
      </div>
      <div class="justify-self-center hover:shadow-md transition duration-500">
        <img src="~/assets/technologies/laravel.svg" />
      </div>
    </div>
  </div>
</template>
