<template>
  <div v-show="loading" class="loader">
      <img class="loader__img" src="../storage/images/logo_transparent.png" alt="mini-tone loader">
  </div>
</template>

<script>
export default {
    data(){
        return{
            loading : true,
        }
    },
    mounted(){
        setTimeout(() => {
            document.querySelector(".loader").classList.add('loader-hidden');
            setTimeout(() => {
                this.loading = false;
            }, 500);
        }, 1500);
    }
}
</script>

<style>
.loader{
    position: fixed;
    background: #1A202C;
    z-index: 999;
    height: 100vh;
    display: flex;
    width: 100vw;
    overflow: show;
    margin: auto;
    top: 0;
    opacity: 1;
    left: 0;
    bottom: 0;
    right: 0;
    justify-content: center;
    align-items: center;
    transition: all 1s cubic-bezier(0.075, 0.82, 0.165, 1);
}
.loader-hidden{
  opacity: 0;
  visibility: hidden;
}
.loader__img{
    width: 500px;
}
</style>