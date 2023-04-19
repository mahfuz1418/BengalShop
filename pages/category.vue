<template>
  <div class="container py-5">
    <div class="flex">
      <div class="w-1/4">
        <Sidebar />
      </div>
      <div class="w-3/4 ml-8">
        <div class="category-bg rounded-2xl">
          <div class="w-1/2 p-10">
            <p class="mb-4 text-xl bs-orange-color">Buy 1 Get 1</p>
            <h3 class="text-4xl font-bold bs-green-color">
              Up to 30% Discount on Selected Items
            </h3>
          </div>
        </div>

        <div class="flex items-center justify-between my-10">
          <h3 class="text-3xl">Category heading</h3>
          <div class="flex items-center min-w-max">
            <div class="mr-6 text-sm"><b>20</b> Products Found</div>
            <select name="" id="">
              <option value="">Default sorting</option>
              <option value="">Sort by price</option>
              <option value="">Sort by discount</option>
            </select>
          </div>
        </div>
        <div class="flex flex-wrap -mx-4">
          <div v-for="item in 9" class="w-1/3 px-4 mb-10">
            <SingleBox :product="item" />
          </div>
        </div>

        <div class="flex justify-center">
          <button class="px-10 py-3 text-white rounded-full bs-green-bg">Load More</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from "../components/Sidebar.vue";
export default {
  components: { Sidebar },
  name: "Category",
};
</script>

<style></style>
