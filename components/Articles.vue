<template>
  <div id="articles" class="bg-blue-200 lg:mt-12">
    <div class="container mx-auto py-1">
      <!-- ARTICLE 1 !-->
      <div
        class="flex flex-col items-center lg:items-start lg:flex-row justify-around relative max-w-6xl my-20 mx-auto"
      >
        <div class="article-image-container shadow">
          <img
            class="object-cover h-full w-full md:rounded"
            alt="Image's Article"
            src="~/assets/images/brigitte.png"
          />
        </div>
        <div class="article-info-container p-5 sm:p-0">
          <h1 class="font-extrabold pt-3 lg:pt-0 text-blue-700 text-3xl">
            Ma (petite) participation au challenge Brigitte Friang
          </h1>
          <span class="text-lg font-light text-blue-700">20.11.2020</span>
          <p class="text-black text-lg mt-2">
            La Direction Générale de la Sécurité Extérieure et l’école ESIEE ont
            organisé un CTF sous le nom de Brigitte Friang en référence à la
            résistante française durant la seconde guerre mondiale.
          </p>
          <a
            href="https://medium.com/@thibeaultchenu/ma-petite-participation-au-challenge-brigitte-friang-f7e54f6d6f61"
            class="text-blue-500 absolute mt-5 lg:bottom-0"
          >
            Lire sur Medium
            <img
              alt="Read more on Medium"
              class="inline"
              src="~/assets/icons/more.svg"
            />
          </a>
        </div>
      </div>

      <!-- ARTICLE 1 !-->
      <div
        class="flex flex-col flex-col-reverse lg:flex-row justify-around relative max-w-6xl my-20 mx-auto"
      >
        <div class="article-info-container p-5 sm:p-0">
          <h1 class="font-extrabold pt-3 lg:pt-0 text-blue-700 text-3xl">
            How did I break a captcha with Puppeteer and Google Vision ?
          </h1>
          <span class="text-lg font-light text-blue-700">01.12.2019</span>
          <p class="text-black text-lg mt-2">
            To prevent robots or users from misusing forms, the implementation
            of a CAPTCHA system is an effective and widespread solution.
          </p>
          <a
            href="https://medium.com/@thibeaultchenu/how-did-i-break-a-captcha-with-puppeteer-and-google-vision-ccde4dde597c"
            class="text-blue-500 absolute mt-5 lg:bottom-0"
          >
            Lire sur Medium
            <img
              alt="Read more on Medium"
              class="inline"
              src="~/assets/icons/more.svg"
            />
          </a>
        </div>
        <div class="article-image-container shadow">
          <img
            class="object-cover h-full w-full md:rounded"
            alt="Image's Article"
            src="https://miro.medium.com/max/700/1*h89l_KJR8w2NrzQXtPCAmw.jpeg"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.article-info-container {
  width: 100%;
}

@media (min-width: 1024px) {
  .article-info-container {
    width: 40%;
  }

  .article-image-container {
    /**
      TODO : refactoring with % ?
     */
    width: 540px;
    height: 300px;
  }
}
</style>
