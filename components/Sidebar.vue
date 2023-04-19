<template>
  <div id="app">
          <accordion >
            <accordion-item class="border-2 border-gray-200 border-soid rounded-xl" :openByDefault="true">
              <!-- This slot will handle the title/header of the accordion and is the part you click on -->
              <template slot="accordion-trigger">
                <h3 class="flex justify-between w-full p-5 cursor-pointer rounded-t-xl" style="background-color: #EBFAEB;">Categories 
                   
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
</svg>


                </h3>
              </template>
              <!-- This slot will handle all the content that is passed to the accordion -->
              <template slot="accordion-content" >
                <div class="accordion-hover">
                  <ul class="ml-4 border-l-2">
                    <li > 
                      <accordion >
                        <accordion-item>
                          <!-- This slot will handle the title/header of the accordion and is the part you click on -->
                          <template slot="accordion-trigger" >
                            <h3 class="flex justify-between w-full py-4 pl-8 pr-5" >Fruits 
                              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
</svg>

                            </h3>
                          </template>
                          <!-- This slot will handle all the content that is passed to the accordion -->
                          <template slot="accordion-content">
                            <ul  class="ml-10 border-l-2">
                              <li class="px-4 py-1 hover:text-green-500"> <nuxt-link to="">Apple</nuxt-link> </li>
                              <li class="px-4 py-1 hover:text-green-500"> <nuxt-link to="">Pineapple</nuxt-link> </li>
                            </ul>
                          </template>
                      </accordion-item>
                      <accordion-item>
                          <!-- This slot will handle the title/header of the accordion and is the part you click on -->
                          <template slot="accordion-trigger">
                            <h3 class="flex justify-between w-full py-4 pl-8 pr-5 ">Vegetable 
                              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
</svg>

                            </h3>
                          </template>
                          <!-- This slot will handle all the content that is passed to the accordion -->
                          <template slot="accordion-content">
                            <ul class="ml-10 border-l-2">
                              <li class="px-4 py-1 hover:text-green-500"><nuxt-link to="">Tomato</nuxt-link> </li>
                              <li class="px-4 py-1 hover:text-green-500"><nuxt-link to="">Potato</nuxt-link> </li>
                            </ul>
                          </template>
                      </accordion-item>
                      <accordion-item>
                          <!-- This slot will handle the title/header of the accordion and is the part you click on -->
                          <template slot="accordion-trigger">
                            <h3 class="flex justify-between w-full py-4 pl-8 pr-5">Cloth 
                              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
</svg>

                            </h3>
                          </template>
                          <!-- This slot will handle all the content that is passed to the accordion -->
                          <template slot="accordion-content">
                            <ul class="ml-10 border-l-2">
                              <li class="px-4 py-1 hover:text-green-500"><nuxt-link to="">Shirt</nuxt-link> </li>
                              <li class="px-4 py-1 hover:text-green-500"><nuxt-link to="">Pant</nuxt-link> </li>
                            </ul>
                          </template>
                      </accordion-item>
                      </accordion>
                    </li>
                  </ul>
                </div>
              </template>
            </accordion-item>

          </accordion>
        </div>
</template>

<script>
import Accordion from '../components/accordion.vue';
import AccordionItem from '../components/accordion-item.vue';

export default {
  name: "App",
  components: {
    Accordion,
    AccordionItem
  }
};
</script>

<style>
</style>