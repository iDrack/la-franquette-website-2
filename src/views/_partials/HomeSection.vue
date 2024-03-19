<template>
  <div class="grid place-content-center">
    <div class="px-4 py-16  mt-16 sm:mt-8 mx-auto sm:max-w-xl md:max-w-full lg:max-w-screen-xl md:px-24 lg:px-8 lg:py-20 ">
        <div class="flex flex-col items-center justify-between w-full mb-10 lg:flex-row">
          <div class="mb-16 lg:mb-0 lg:max-w-lg">
            <div class="max-w-xl mb-6">
              <h3 class="color-primary lato-regular">
                La bonne Franquette
              </h3>
              <h2 class="max-w-lg mb-6 text-3xl sm:text-4xl sm:leading-none">
                <span class="font-bold">
                  La caisse facile
                </span> 
                <br class="hidden md:block" />
                <span class="inline-block">
                  pour des journées plus fluides
                </span>
              </h2>
              <p class="text-base md:text-lg">
                Transformez votre tablette en une caisse intelligente avec notre application sur mesure.
                Du food truck au stand de marché, notre application s'adapte à votre menu. 
              </p>
            </div>
          </div>
          <div class="flex items-center justify-center lg:w-1/2 pl-4 ml-16">
              <div class="w-8/12 z-30 -mr-16 lg:-ml-32">
                  <img class="object-cover" src="/ressources/img/photo-home2.png" alt="Tablette montrant le logiciel de caisse La bonne Franquette" />
                </div>
                <div class="w-10/12 -ml-16 lg:-ml-32 pt-4">
                  <img class="object-cover" src="/ressources/img/photo-home.png" alt="Tablette montrant la page de connexion au logiciel La bonne Franquette" />
                </div>
          </div>
        </div>
    </div>
    <div class="w-full md:flex items-center justify-center sm:hidden">
      <a href="#product" class="smooth">
        <ChevronDownIcon 
            href="#product"
            aria-label="Scroll down" 
            class="size-10 color-primary border-2 border-gray-100 rounded-full p-2 hover:shadow" />    
        </a>
        </div>

  </div>


</template>

<style scoped>

</style>
<script setup>
  import { ChevronDownIcon } from '@heroicons/vue/24/outline';

  function scrollToProductionSection() {

  }

</script>
