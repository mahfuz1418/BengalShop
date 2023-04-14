<template>
  <div class="container">
    <div class="flex">
      <div class="w-1/4">
        <sidebar/>
      </div>
      <div class="w-3/4">main bar</div>
    </div>
  </div>
</template>

<script>
import Sidebar from '../components/Sidebar.vue';
export default {
  components: { Sidebar },
  name: "Category",
};
</script>

<style>
</style>
