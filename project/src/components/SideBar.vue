<template>
      <div class="sidebar py-4 w-20 top-5 my-20 px-2 text-gray-700 bg-gray-900 rounded text-center shadow-lg">
       <img src="../storage/images/logo_transparent.png"
            alt="MINI-TONE" class="navbar__logo inline mx-auto">
        <span class="cursor-pointer hover:text-white px-2 block mb-5">
          <i class="fas fa-stream">
          </i>
        </span>
        <span class="cursor-pointer hover:text-white px-2 block mb-5">
          <i class="fas fa-search p-2 bg-gray-800 rounded-full">
          </i>
        </span>
     
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .sidebar{
        position: relative;
        left: -5%;
        transition: all 0.5s cubic-bezier(0.075, 0.82, 0.165, 1);
    }
    .sidebar:hover{
        left: 0;
    }
</style>