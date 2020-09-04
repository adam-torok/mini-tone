<template>
  <div>
    <NavBar></NavBar>
    <SideBar></SideBar>
    <div class="song__holder">
      <div v-for="song in songs" :key="song.id">
        <MusicCard :songs="song"></MusicCard>
      </div>
    </div>
  <Player></Player>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import SideBar from '@/components/SideBar'
import Player from '@/components/Player'
import MusicCard from '@/components/MusicCard';
export default {
    components:{
        MusicCard,
        SideBar,
        NavBar,
        Player
    },
    data(){
        return{
            songs:[
                {name:'Artist',
                artist:'artist'},
                {name:'Artist2',
                artist:'artist2'},
                {name:'Artist3',
                artist:'artist3'},
                {name:'Artist',
                artist:'artist'},
                {name:'Artist2',
                artist:'artist2'},
                {name:'Artist3',
                artist:'artist3'},
            ]
        }
    }
}
</script>

<style>
.song__holder{
    margin: 1.5rem;
    margin-top: 3rem;
    justify-content: center;
    align-content: center;
    align-items: center;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-gap: 30px;
}
</style>