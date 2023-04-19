<template>
  <div>
    <div class="container">
      <div class="flex -mx-4 py-20">
        <div class="w-1/4 flex items-center mx-2">
          <div class="min-w-max mr-4">
            <img
              width="80px"
              height="80px"
              src="~/assets/img/callcenter.png"
              alt=""
            />
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">24 Customer Support</h3>
            <p class="text-gray-500">Contact us 24 hours</p>
          </div>
        </div>

        <div class="w-1/4 flex items-center mx-2">
          <div class="min-w-max mr-4">
            <img
              width="80px"
              height="80px"
              src="~/assets/img/products.png"
              alt=""
            />
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">Authentic Products</h3>
            <p class="text-gray-500">Contact us 24 hours</p>
          </div>
        </div>

        <div class="w-1/4 flex items-center mx-2">
          <div class="min-w-max mr-4">
            <img
              width="80px"
              height="80px"
              src="~/assets/img/payments.png"
              alt=""
            />
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">24 Secure Payment</h3>
            <p class="text-gray-500">Contact us 24 hours</p>
          </div>
        </div>

        <div class="w-1/4 flex items-center mx-2">
          <div class="min-w-max mr-4">
            <img
              width="80px"
              height="80px"
              src="~/assets/img/offers.png"
              alt=""
            />
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">Best Prices & Offers</h3>
            <p class="text-gray-500">Contact us 24 hours</p>
          </div>
        </div>
      </div>
    </div>

    <div class="pt-20 pb-10" style="background-color: #f5f5f5">
      <div class="container">
        <div class="flex items-start pb-10">
          <div class="w-3/6">
            <Logo />
            <p class="my-10">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Velit
              explicabo ipsam dolores. Tempore fugiat maxime blanditiis
              molestias velit beatae labore quae, explicabo voluptates iste nam,
              cumque facilis
            </p>

            <div class="flex">
              <a href="/" class="mr-3"
                ><img src="~/assets/img/appstore.png" alt=""
              /></a>
              <a href="/"><img src="~/assets/img/playstore.png" alt="" /></a>
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
              <a href="" class="pr-1"
                ><img
                  class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white"
                  src="~/assets/img/facebook.png"
                  alt=""
              /></a>
              <a href="" class="px-1"
                ><img
                  class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white"
                  src="~/assets/img/instagram.png"
                  alt=""
              /></a>
              <a href="" class="px-1"
                ><img
                  class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white"
                  src="~/assets/img/twitter.png"
                  alt=""
              /></a>
              <a href="" class="px-1"
                ><img
                  class="p-4 w-12 h-12 bg-white hover:bg-orange-400 rounded hover:text-white"
                  src="~/assets/img/skype.png"
                  alt=""
              /></a>
            </div>
          </div>
          <div class="w-2/6">
            <small class="text-gray-500"
              >@2022 Copyright All Right Reserved by Bengal Shop</small
            >
          </div>
          <div class="w-2/6">
            <img
              class="w-72 ml-auto"
              src="~/assets/img/paymentoption.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>

    <!-- PRODUCT DETAILS MODAL  -->
    <div v-if="modal" class="fixed w-full h-full top-0 left-0 z-30">
      <div  @click.prevent="modalClose"
        class="absolute bg-black opacity-60 h-full w-full top-0 left-0"
      ></div>
      <div
        class="bs-modal-body bg-white rounded-2xl z-30 relative mx-auto mt-20"
      >
        <div class="top-4 right-4 absolute">
          <svg @click.prevent="modalClose"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-5 h-5 cursor-pointer hover:text-green-600"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6 18L18 6M6 6l12 12"
            />
          </svg>
        </div>
        <div class="flex p-8">
          <div class="w-1/2 pr-4">
            <img src="~/assets/img/kata_tomato.png" alt="" />
          </div>
          <div class="w-1/2 pl-4">
            <div class="flex font-medium text-base">
              <h4 class="text-gray-500">STATUS</h4>
              <h4 class="ml-8 text-green-600">in Stock</h4>
            </div>
            <h3 class="text-2xl font-medium my-2">
              Product Full Name Here.... -{{ product }}
            </h3>
            <p class="font-size-14 text-gray-500"><b>7</b> item available</p>
            <div class="flex items-center my-4">
              <h3 class="text-3xl font-bold">$59.00</h3>
              <h4 class="text-2xl ml-3 text-gray-500 flex items-center">
                <del>$69.00</del
                ><small class="font-size-14 ml-3">(+15% Vat Included)</small>
              </h4>
            </div>
            <hr />



            <div class="text-gray z-10">
              <div
                class="flex items-center justify-center h-full text-3xl my-4"
              >
                <button
                  class="p-5 hover:text-green-500 w-8 h-8 text-base font-bold rounded-full border-solid border-gray border-2 flex justify-center items-center"
                >
                  -
                </button>
                <span
                  class="p-5 mx-4 w-8 h-8 text-base font-bold rounded-full border-solid border-gray bg-gray-100 border-2 flex justify-center items-center "
                  >1</span
                >
                <button
                  class="p-5 hover:text-green-500 w-8 h-8 text-base font-bold rounded-full border-solid border-gray border-2 flex justify-center items-center"
                >
                  +
                </button>
              </div>
              <button
                class="bs-green-bg px-10 py-3 rounded-full text-white w-full hover:bg-green-600"
              >
                Add To Cart
              </button>
              <button
                class="bg-gray-100 px-10 py-3 rounded-full w-full my-3 hover:bg-gray-200"
              >
                Buy Now
              </button>
            </div>


            <div class="flex justify-between my-2">
              <div class="flex items-center">
                <img style="width: 16px; height: 16px;" class="mr-2 cursor-pointer" src="~/assets/img/icon.png" alt=""> 
                <p class="font-size-14 text-gray-500">Add to Wishlist</p>
              </div>
              <div class="flex items-center">
                <img style="width: 16px; height: 17px;" class="mr-2 cursor-pointer" src="~/assets/img/share.png" alt=""> 
                <p class="font-size-14 text-gray-500">Add to Wishlist</p>
              </div>
            </div>
            <hr class="my-2">

            <div class="leading-loose">
              <p class="font-size-14"><span class=" font-medium text-gray-500 w-40 inline-block">CATEGORY</span>Food</p>
              <p  class="font-size-14"><span class=" font-medium text-gray-500 w-40 inline-block">TAGS</span>Food, Fruits, Vegetables</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      modal: false,
      product: ''
    }
  },
  methods: {
    modalClose() {
      this.modal = false;
      this.$store.dispatch("product-details-modal/resetModal");
    }
  },
  mounted() {
    this.$store.watch(
      () => {
        return this.$store.getters["product-details-modal/getModal"]
      },
      (val)=>{
        this.modal = val.modal
        this.product = val.product
      },
      {
        deep:true
      }
    );
  }
};
</script>

<style scoped></style>
