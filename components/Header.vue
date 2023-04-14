<template>
  <div class="container">
    <div class="flex justify-between items-center py-6">
      <div class="min-w-max">
        <Logo/>
      </div>
      <div class="w-96">
        <div class="border border-gray-300 flex p-0.5 rounded-full items-center">
          <div class="min-w-max px-3">
            <img src="~/assets/img/search.png" alt="">
          </div>
          <input class="w-full focus:outline-none px-3 py-1" type="search" name="" id="" placeholder="Search Here.....">
          <button type="submit" class="bs-button-bg px-4 py-1 rounded-full text-white">Search</button>
        </div>
      </div>

      <div class="min-w-max flex items-center">
        <nuxt-link to=""><span class="bs-icon-box hover:bg-gray-200 inline-block rounded-full flex items-center justify-center"><img src="~/assets/img/heart.png" alt=""></span></nuxt-link>
        <nuxt-link to="" class="relative"><span class="bs-icon-box hover:bg-gray-200 inline-block rounded-full flex items-center justify-center"><img src="~/assets/img/shopping-beg.png" alt=""></span><span class="absolute top-0 right-0 bg-red-600 w-4 h-4 rounded-full text-xs flex items-center justify-center text-white">0</span></nuxt-link>
        <nuxt-link to="" class="flex items-center"><span class="bs-icon-box hover:bg-gray-200 inline-block rounded-full flex items-center justify-center"><img src="~/assets/img/avater.png" alt=""></span><span>Account</span></nuxt-link>
      </div>
    </div>


    <div class="flex items-center">
      <div  class="w-96 relative ">
        <div v-click-outside="onClickOutside" @click.prevent="menuClick" class="bs-green-bg flex px-4 py-2 rounded-full items-center cursor-pointer relative z-20">
          <div class="min-w-man">
            <img src="~/assets/img/menu-right.png" alt="">
          </div>
          <div class="w-full text-white text-center px-6">
            All Categories
          </div>
          <div class="min-w-man">
            <img src="~/assets/img/chevron-down.png" alt="">
          </div>
        </div>
        <div v-bind:class=" CategoryMenu ? 'block visible'  : 'hidden invisible' " class=" absolute z-10 text-center w-full bs-green-bg -mt-4 rounded-b-2xl">
          <ul class="mt-5 text-white">
            <li class="py-1.5"><nuxt-link to="/">Home</nuxt-link></li>
            <li class="py-1.5"><nuxt-link to="/category">Category</nuxt-link></li>
            <li class="py-1.5"><nuxt-link to="/">Aboute</nuxt-link></li>
            <li class="py-1.5"><nuxt-link to="/">Contact</nuxt-link></li>
            <li class="py-1.5"><nuxt-link to="/">Blog</nuxt-link></li>
            <li class="py-1.5"><nuxt-link to="/">Shop</nuxt-link></li>
            <li class="py-1.5"><nuxt-link to="/">Track Offer</nuxt-link></li>
          </ul>
      </div>
      </div>
      <div class="w-full">
        <ul class="flex justify-center">
          <li><nuxt-link class="p-4" to="/">Home</nuxt-link></li>
          <li><nuxt-link class="p-4" to="/category">Category</nuxt-link></li>
          <li><nuxt-link class="p-4" to="">Pages</nuxt-link></li>
          <li><nuxt-link class="p-4" to="">Blogs</nuxt-link></li>
          <li><nuxt-link class="p-4" to="">Contact</nuxt-link></li>
          <li><nuxt-link class="p-4" to="">Track Offer</nuxt-link></li>
        </ul>
      </div>
      <div class="min-w-max flex items-center bs-orange-color">
        <img class="mr-3 w-4 h-4" src="~/assets/img/persent.png" alt=""> Special Offers!
      </div>
    </div>
    
    
  </div>

</template>

<script>
export default {
  name: 'Header',

  data() {
    return {
      CategoryMenu : false
    }
  },

  methods: {
    menuClick() {
      this.CategoryMenu = !this.CategoryMenu ;
    },
    onClickOutside() {
      this.CategoryMenu = false ;
    }
  }
}

</script>

<style scoped>

</style>