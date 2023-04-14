<template>
  <div>
    <!-- START HERO SLIDER SECTION  -->
    <div class="p-6 hero-slider">
      <vue-slick-carousel :arrows="false" :dots="true">
        <div class="slider-bg rounded-2xl">
          <div class="container pt-10 px-10">
            <div class="flex">
              <div class="w-1/2 my-auto">
                <p class="text-3xl bs-green-color">Save up 30% off</p>
                <h2 class="font-size-70 font-bold py-5">
                  Bengal Vegetable farm Organic 100%
                </h2>
                <p class="mb-10">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Vehicula faucibus massa est elit maecenas.
                </p>
                <nuxt-link
                  to="/"
                  class="bs-green-bg px-8 py-2 rounded-full text-white"
                  >Shop Now</nuxt-link
                >
              </div>
              <div class="w-1/2 flex justify-end">
                <img width="450px" src="~/assets/img/hero.png" alt="" />
              </div>
            </div>
          </div>
        </div>

        <div class="slider-bg rounded-2xl">
          <div class="container pt-10 px-10">
            <div class="flex">
              <div class="w-1/2 my-auto">
                <p class="text-3xl bs-green-color">Save up 30% off</p>
                <h2 class="font-size-70 font-bold py-5">
                  Bengal Vegetable farm Organic 80%
                </h2>
                <p class="mb-10">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Vehicula faucibus massa est elit maecenas.
                </p>
                <nuxt-link
                  to="/"
                  class="bs-green-bg px-8 py-2 rounded-full text-white"
                  >Shop Now</nuxt-link
                >
              </div>
              <div class="w-1/2 flex justify-end">
                <img width="450px" src="~/assets/img/hero.png" alt="" />
              </div>
            </div>
          </div>
        </div>

        <div class="slider-bg rounded-2xl">
          <div class="container pt-10 px-10">
            <div class="flex">
              <div class="w-1/2 my-auto">
                <p class="text-3xl bs-green-color">Save up 30% off</p>
                <h2 class="font-size-70 font-bold py-5">
                  Bengal Vegetable farm Organic 50%
                </h2>
                <p class="mb-10">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Vehicula faucibus massa est elit maecenas.
                </p>
                <nuxt-link
                  to="/"
                  class="bs-green-bg px-8 py-2 rounded-full text-white"
                  >Shop Now</nuxt-link
                >
              </div>
              <div class="w-1/2 flex justify-end">
                <img width="450px" src="~/assets/img/hero.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </vue-slick-carousel>
      <!-- END HERO SLIDER SECTION  -->

      <!-- START CATEGORY SLIDER SECTION  -->
      <div class="container pt-20">
        <h3 class="text-3xl font-semibold mb-10">Search by Category</h3>
        <div class="flex items-center">
          <div style="height: 4px" class="w-32 bs-green-bg rounded"></div>
          <div style="height: 2px" class="w-full bg-gray-200"></div>
        </div>

        <vue-slick-carousel
          class="category-carousel py-10 -ml-2 -mr-6"
          v-bind="CategoryCarouselSetting"
        >
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 mr-0 flex justify-center items-center">
              <img src="~/assets/img/category(1).png" alt="" />
            </div>
            <h4 class="text-center">Ice Cream</h4>
          </div>
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/category(2).png" alt="" />
            </div>
            <h4 class="text-center">Fruits</h4>
          </div>
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/category(3).png" alt="" />
            </div>
            <h4 class="text-center">Vegetables</h4>
          </div>
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/category(4).png" alt="" />
            </div>
            <h4 class="text-center">Fish</h4>
          </div>
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/category(5).png" alt="" />
            </div>
            <h4 class="text-center">Meat</h4>
          </div>
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/category(6).png" alt="" />
            </div>
            <h4 class="text-center">Groceries</h4>
          </div>
          <div class="bg-gray-200 p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/category(5).png" alt="" />
            </div>
            <h4 class="text-center">meat</h4>
          </div>
          <template #prevArrow="arrowOption">
            <div class="custom-arrow">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 left"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15.75 19.5L8.25 12l7.5-7.5"
                />
              </svg>
            </div> </template
          ><template #nextArrow="arrowOption">
            <div class="custom-arrow">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 right"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M8.25 4.5l7.5 7.5-7.5 7.5"
                />
              </svg>
            </div>
          </template>
        </vue-slick-carousel>
      </div>
      <!-- END CATEGORY SLIDER SECTION  -->

      <!-- START PROMO-BG SLIDER SECTION  -->
      <div class="container">
        <div class="flex -mx-6 pt-14">
          <div class="w-1/2 mx-4">
            <div class="promo-bg-1 bg-gray-300 px-12 py-20 rounded-2xl">
              <div class="w-1/2">
                <p class="text-xl bs-orange-color mb-4">Buy 1 Get 1</p>
                <h3 class="text-4xl font-bold mb-10 leading-normal">
                  Fresh Fruits Collection
                </h3>
                <nuxt-link
                  to="/"
                  class="bg-white px-8 py-2 rounded-full bs-orange-color"
                  >Shop Now</nuxt-link
                >
              </div>
            </div>
          </div>
          <div class="w-1/2 mx-4">
            <div class="promo-bg-2 bg-gray-300 px-12 py-20 rounded-2xl">
              <div class="w-1/2">
                <p class="text-xl bs-orange-color mb-4">Buy 1 Get 1</p>
                <h3 class="text-4xl font-bold mb-10 leading-normal">
                  Fresh Fruits Collection
                </h3>
                <nuxt-link
                  to="/"
                  class="bg-white px-8 py-2 rounded-full bs-orange-color"
                  >Shop Now</nuxt-link
                >
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- END PROMO-BG SLIDER SECTION  -->

      <!-- START PRODUCT SLIDER SECTION  -->
      <div class="container pt-20">
        <h3 class="text-3xl font-semibold mb-10">Deals of the Week</h3>
        <div class="flex items-center">
          <div style="height: 4px" class="w-32 bs-green-bg rounded"></div>
          <div style="height: 2px" class="w-full bg-gray-200"></div>
        </div>

        <vue-slick-carousel
          class="category-carousel py-10 -ml-2 -mr-6"
          v-bind="Setting"
        >
          <SingleBox v-for="item in 10" :product="item"/>

          <template #prevArrow="arrowOption">
            <div class="custom-arrow">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 left"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15.75 19.5L8.25 12l7.5-7.5"
                />
              </svg>
            </div> </template
          ><template #nextArrow="arrowOption">
            <div class="custom-arrow">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 right"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M8.25 4.5l7.5 7.5-7.5 7.5"
                />
              </svg>
            </div>
          </template>
        </vue-slick-carousel>
      </div>
      <!-- END PRODUCT SLIDER SECTION  -->

      <!-- START BRAND SLIDER SECTION  -->
      <div class="container pt-20">
        <h3 class="text-3xl font-semibold mb-10">Popular Brands</h3>
        <div class="flex items-center">
          <div style="height: 4px" class="w-32 bs-green-bg rounded"></div>
          <div style="height: 2px" class="w-full bg-gray-200"></div>
        </div>

        <vue-slick-carousel
          class="category-carousel py-10 -ml-2 -mr-6"
          v-bind="CategoryCarouselSetting"
        >
          <div class="p-4 rounded">
            <div class="h-28 mr-0 flex justify-center items-center">
              <img src="~/assets/img/frame-1.png" alt="" />
            </div>
          </div>
          <div class="p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/frame-5.png" alt="" />
            </div>
          </div>
          <div class="p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/frame-2.png" alt="" />
            </div>
          </div>
          <div class="p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/frame-3.png" alt="" />
            </div>
          </div>
          <div class="p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/frame-4.png" alt="" />
            </div>
          </div>
          <div class="p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/frame-5.png" alt="" />
            </div>
          </div>
          <div class="p-4 rounded">
            <div class="h-28 flex justify-center items-center">
              <img src="~/assets/img/frame-6.png" alt="" />
            </div>
          </div>
          <template #prevArrow="arrowOption">
            <div class="custom-arrow">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 left"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15.75 19.5L8.25 12l7.5-7.5"
                />
              </svg>
            </div> </template
          ><template #nextArrow="arrowOption">
            <div class="custom-arrow">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6 right"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M8.25 4.5l7.5 7.5-7.5 7.5"
                />
              </svg>
            </div>
          </template>
        </vue-slick-carousel>
      </div>
      <!-- END BRAND SLIDER SECTION  -->

      <!-- START PROMO-BG SLIDER SECTION  -->
      <div class="container">
        <div class="flex -mx-6 pt-14">
          <div class="w-1/3 mx-4">
            <div
              class="p-8 rounded-2xl flex items-center"
              style="background-color: #fff0dc"
            >
              <div class="w-1/2">
                <h3 class="text-xl font-bold mb-14 leading-normal">
                  Fresh Fruits Collection
                </h3>
                <nuxt-link
                  to="/"
                  class="bg-white p-2 rounded-full bs-orange-color"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 inline"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3"
                    /></svg
                ></nuxt-link>
              </div>
              <div class="w-1/2">
                <img src="~/assets/img/pineaple.png" alt="" />
              </div>
            </div>
          </div>
          <div class="w-1/3 mx-4">
            <div
              class="p-8 rounded-2xl flex items-center"
              style="background-color: #ddf1d6"
            >
              <div class="w-1/2">
                <h3 class="text-xl font-bold mb-14 leading-normal">
                  Fresh Fruits Collection
                </h3>
                <nuxt-link
                  to="/"
                  class="bg-white p-2 rounded-full bs-orange-color"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 inline"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3"
                    /></svg
                ></nuxt-link>
              </div>
              <div class="w-1/2">
                <img src="~/assets/img/tomato.png" alt="" />
              </div>
            </div>
          </div>
          <div class="w-1/3 mx-4">
            <div
              class="p-8 rounded-2xl flex items-center"
              style="background-color: #ffebb7"
            >
              <div class="w-1/2">
                <h3 class="text-xl font-bold mb-14 leading-normal">
                  Fresh Fruits Collection
                </h3>
                <nuxt-link
                  to="/"
                  class="bg-white p-2 rounded-full bs-orange-color"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-6 h-6 inline"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3"
                    /></svg
                ></nuxt-link>
              </div>
              <div class="w-1/2">
                <img src="~/assets/img/packet.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- END PROMO-BG SLIDER SECTION  -->
    </div>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "IndexPage",
  components: { Header, Footer },
  data() {
    return {
      CategoryCarouselSetting: {
        slidesToShow: 6,
      },
      Setting: {
        slidesToShow: 4,
      },
    };
  },
};
</script>
