<template>
<div>
    {{song}}
<div class="music__card bg-gray-900 rounded rounded-t-lg overflow-hidden shadow max-w-xs my-3">
<div class="flex justify-center">
    <img src="../storage/images/logo.png" class="music__card-album w-20 border-solid border-white border-2 -mt-3">		
</div>
<div class="text-center px-3 py-4">
    <h3 class="text-teal-400 text-sm bold font-sans">Olivia Dunham</h3>
    <p class="mt-2 font-sans font-light text-gray-600">Hello, i'm from another the other side!</p>
    <div class="text-grey-darker">
        <i class="text-teal-400 fas mt-5 fa-play fa-xl"></i>
    </div>
</div>
</div>
</div>
</template>

<script>
export default {
props:['song'],
}
</script>

<style>
.music__card{
  overflow: inherit;
}
.music__card-album{
    height: 5rem;
}
</style>