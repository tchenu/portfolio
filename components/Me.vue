<template>
  <div
    class="container mx-auto mt-0 md:mt-24 p-8 rounded-lg bg-blue-100 items-center"
  >
    <div class="flex justify-between items-center">
      <div>
        <h1 class="font-light text-3xl">Hello 👋🏻</h1>
        <h1 class="text-blue-600 font-extrabold text-3xl leading-3">
          Thibeault
        </h1>
        <br />
        <br />
        <p class="font-regular text-xl max-w-md">
          I am a student at
          <span class="text-blue-500">@ESGI</span>
          in 4th year of web engineering.
          <br />
          <br />

          I'm currently in apprenticeship as
          <span class="text-blue-500">full-stack developer</span> at
          <span class="text-blue-500">@SVP</span>.
          <br />
          <br />

          I'm also a
          <span class="text-blue-500">hacker</span>
          at night and on weekends.
          <br />
          <br />
        </p>
      </div>
      <div class="hidden md:block">
        <img
          alt="Image represents my 4 tech profiles"
          src="~/assets/images/me.svg"
        />
      </div>
    </div>
    <div>
      <a
        id="hire-me"
        class="inline-block shadow-xl px-10 py-3 text-white text-center bg-blue-600 rounded-md font-semibold align-middle"
        href="https://www.malt.fr/profile/thibeaultchenu"
      >
        Hire me
      </a>
      <NuxtLink
        id="cv"
        to="/cv"
        class="inline-block px-5 py-3 text-white text-center bg-blue-700 rounded-md mx-5 font-semibold align-middle"
      >
        CV
      </NuxtLink>
    </div>
  </div>
</template>
