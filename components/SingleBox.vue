<template>
  <div class="text-center product">
            <div class="h-80 relative">
              <div
                class="bg-gray-200 p-0 rounded h-80 mr-0 flex justify-center items-center"
              >
                <img src="~/assets/img/pineaple.png" alt="" />
              </div>
              <div
                class="product-hover absolute top-0 left-0 h-full w-full flex justify-center items-center"
              >
                <div class="bg-black absolute w-full h-full opacity-50"></div>
                <nuxt-link
                  class="absolute left-0 bottom-0 flex items-center justify-center w-full bg-gray-200 text-gray-600 py-1.5"
                  to=""
                  >Details
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-4 h-4"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M4.5 12h15m0 0l-6.75-6.75M19.5 12l-6.75 6.75"
                    />
                  </svg>
                </nuxt-link>
                <div class="text-white z-10">
                  <div
                    class="flex items-center justify-center h-full text-3xl my-4"
                  >
                    <button
                      class="p-6 w-10 h-10 rounded-full border-solid border-white border-2 flex justify-center items-center"
                    >
                      -
                    </button>
                    <span
                      class="p-6 mx-4 w-10 h-10 rounded-full border-solid border-white bs-green-bg border-2 flex justify-center items-center"
                      >1</span
                    >
                    <button
                      class="p-6 w-10 h-10 rounded-full border-solid border-white border-2 flex justify-center items-center"
                    >
                      +
                    </button>
                  </div>
                  <button class="bs-green-bg px-10 py-3 rounded-full">
                    Add To Cart
                  </button>
                </div>
              </div>
            </div>
            <h4 class="text-center text-sm mt-5 text-gray-400">
              Category Name
            </h4>
            <h3 class="text-xl font-medium my-4">Product Name - {{ product }}</h3>
            <p class="flex items-center justify-center">
              <span class="bs-orange-color mx-2 text-xl font-medium"
                >$200.00</span
              ><del class="text-gray-400 mx-2">$300.00</del>
            </p>
          </div>
</template>

<script>
    export default {
        name : 'SingleBox',
        props : ['product'], 
    }
</script>

<style>

</style>