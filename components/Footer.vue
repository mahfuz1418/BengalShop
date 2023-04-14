<template>
    <div>
      <div class="container">
        <div class="flex -mx-4 py-20">
          <div class="w-1/4 flex items-center mx-2">
            <div class="min-w-max mr-4">
              <img width="80px" height="80px" src="~/assets/img/callcenter.png" alt="">
            </div>
            <div class="w-full">
              <h3 class="text-xl font-medium mb-2">24 Customer Support</h3>
              <p class="text-gray-500">Contact us 24 hours</p>
            </div>
          </div>

          <div class="w-1/4 flex items-center mx-2">
            <div class="min-w-max mr-4">
              <img width="80px" height="80px" src="~/assets/img/products.png" alt="">
            </div>
            <div class="w-full">
              <h3 class="text-xl font-medium mb-2">Authentic Products</h3>
              <p class="text-gray-500">Contact us 24 hours</p>
            </div>
          </div>

          <div class="w-1/4 flex items-center mx-2">
            <div class="min-w-max mr-4">
              <img width="80px" height="80px" src="~/assets/img/payments.png" alt="">
            </div>
            <div class="w-full">
              <h3 class="text-xl font-medium mb-2">24 Secure Payment</h3>
              <p class="text-gray-500">Contact us 24 hours</p>
            </div>
          </div>

          <div class="w-1/4 flex items-center mx-2">
            <div class="min-w-max mr-4">
              <img width="80px" height="80px" src="~/assets/img/offers.png" alt="">
            </div>
            <div class="w-full">
              <h3 class="text-xl font-medium mb-2">Best Prices & Offers</h3>
              <p class="text-gray-500">Contact us 24 hours</p>
            </div>
          </div> 
        </div>
      </div>


      <div class="pt-20 pb-10" style="background-color: #F5F5F5;">
        <div class="container">
          <div class="flex items-start pb-10">
            <div class="w-3/6 ">
              <Logo/>
              <p class="my-10">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Velit explicabo ipsam dolores. Tempore fugiat maxime blanditiis molestias velit beatae labore quae, explicabo voluptates iste nam, cumque facilis</p>

              <div class="flex">
                <a href="/" class="mr-3"><img src="~/assets/img/appstore.png" alt=""></a>
                <a href="/"><img src="~/assets/img/playstore.png" alt=""></a>
              </div>
            </div>
            <div class="w-1.5/6 ml-20">
              <h3 class="text-xl font-medium mb-2">About Us</h3>
              <ul class="leading-10 mt-6">
                <li><nuxt-link to="/">About Karte</nuxt-link></li>
                <li><nuxt-link to="/">Contact</nuxt-link></li>
                <li><nuxt-link to="/">Career</nuxt-link></li>
                <li><nuxt-link to="/">Terms & Condition</nuxt-link></li>
                <li><nuxt-link to="/">Category</nuxt-link></li>
              </ul>
            </div>
            <div class="w-1.5/6 ml-20">
              <h3 class="text-xl font-medium mb-2">Info</h3>
              <ul class="leading-10 mt-6">
                <li><nuxt-link to="/">Information</nuxt-link></li>
                <li><nuxt-link to="/">Shipping</nuxt-link></li>
                <li><nuxt-link to="/">Payment</nuxt-link></li>
                <li><nuxt-link to="/">Return</nuxt-link></li>
                <li><nuxt-link to="/">Blog</nuxt-link></li>
              </ul>
            </div>
          </div>

          <div class="flex justify-between mt-20 items-center">
            <div class="w-2/6">
              <div class="flex">
                <a href="" class="pr-1"><img class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white" src="~/assets/img/facebook.png" alt=""></a>
                <a href="" class="px-1"><img class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white" src="~/assets/img/instagram.png" alt=""></a>
                <a href="" class="px-1"><img class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white" src="~/assets/img/twitter.png" alt=""></a>
                <a href="" class="px-1"><img class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white" src="~/assets/img/skype.png" alt=""></a>
              </div>
            </div>
            <div class="w-2/6">
              <small class="text-gray-500">@2022 Copyright All Right Reserved by Bengal Shop</small>
            </div>
            <div class="w-2/6">
              <img class="w-72 ml-auto" src="~/assets/img/paymentoption.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  
  </style>