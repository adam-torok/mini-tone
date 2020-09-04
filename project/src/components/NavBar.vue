<template>
 <div class="navbar p-2 m-2 text-gray-700 bg-gray-900 rounded-lg shadow-lg">
        <router-link to="/Home">
          <span class="px-2 mr-2 border-r border-gray-800">
            <img src="../storage/images/logo_transparent.png"
              alt="MINI_TONE" class="navbar__logo inline mx-auto">
          </span>
        </router-link>
        <router-link to="Profile">
          <span class="px-1 hover:text-white cursor-pointer">
          <i class="fas fa-user p-2 bg-gray-800 rounded-full"></i>
          </span>
        </router-link>
        <span class="px-1 hover:text-white cursor-pointer">
          <i class="fas fa-search p-2 bg-gray-800 rounded-full">
          </i>
        </span>
        <span class="px-1 hover:text-white cursor-pointer">
          <i class="w-8 fas fa-calendar-alt p-2 bg-gray-800 rounded-full">
          </i>
        </span>
        <span class="px-1 hover:text-white cursor-pointer w-8 relative">
          <i class="fas fa-bell p-2 bg-gray-800 rounded-full">
          </i>
          <span
            class="absolute right-0 top-0 -mt-2 -mr-1 text-xs bg-red-500 text-white font-medium px-2 shadow-lg rounded-full">3</span>
        </span>
      </div>
</template>

<script>
export default {

}
</script>

<style>
.navbar{
  position: sticky;
  top: 1px;
}
.navbar__logo{
    width:3.5rem;
}
</style>