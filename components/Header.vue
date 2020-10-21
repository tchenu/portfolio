<template>
  <header class="container mx-auto">
    <!-- DESKTOP NAV !-->
    <nav class="hidden sm:flex sm:justify-between sm:items-center sm:h-24">
      <div class="left">
        <NuxtLink to="/" class="pr-6 font-medium text-blue-700 md:text-lg">
          🏠
        </NuxtLink>
        <a class="px-6 font-medium text-blue-700 md:text-lg" href="/#skills">
          Skills
        </a>
        <a
          class="px-6 font-medium text-blue-700 md:text-lg"
          href="https://github.com/tchenu"
        >
          Code
        </a>
        <a class="px-6 font-medium text-blue-700 md:text-lg" href="/#articles">
          Articles
        </a>
      </div>
      <div class="right flex items-center">
        <a class="px-3" href="https://github.com/tchenu">
          <img alt="Github Icon" src="~/assets/icons/github.svg" />
        </a>
        <a class="px-3" href="https://twitter.com/thibeault_chenu">
          <img alt="Twitter Icon" src="~/assets/icons/twitter.svg" />
        </a>
        <a class="px-3" href="https://www.malt.fr/profile/thibeaultchenu">
          <img alt="Malt Icon" src="~/assets/icons/malt.svg" />
        </a>
        <a class="px-3" href="mailto:hello@tchenu.com">
          <img alt="Mail Icon" src="~/assets/icons/mail.svg" />
        </a>
      </div>
    </nav>
    <!-- MOBILE NAV !-->
    <nav class="flex justify-around items-center h-24 sm:hidden">
      <div class="left">
        <NuxtLink to="/" class="pr-6 font-medium text-blue-700 md:text-lg">
          🏠
        </NuxtLink>
        <a
          class="px-6 font-medium text-blue-700 md:text-lg"
          href="https://github.com/tchenu"
        >
          Github
        </a>
        <a class="px-6 font-medium text-blue-700 md:text-lg" href="/#articles">
          Articles
        </a>
      </div>
      <div class="right flex items-center">
        <a class="px-3" href="https://github.com/tchenu">
          <img alt="Github Icon" src="~/assets/icons/github.svg" />
        </a>
        <a class="px-3" href="https://twitter.com/thibeault_chenu">
          <img alt="Twitter Icon" src="~/assets/icons/twitter.svg" />
        </a>
        <a class="px-3" href="https://www.malt.fr/profile/thibeaultchenu">
          <img alt="Malt Icon" src="~/assets/icons/malt.svg" />
        </a>
        <a class="px-3" href="mailto:hello@tchenu.com">
          <img alt="Mail Icon" src="~/assets/icons/mail.svg" />
        </a>
      </div>
    </nav>
  </header>
</template>

<style>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
}
</style>
