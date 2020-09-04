<template>
  <div>
    <Loader></Loader>
    <NavBar></NavBar>
    <SideBar></SideBar>
    <div class="song__holder">
      <div v-for="song in songs" :key="song.id">
        <MusicCard @clicked="playSong" :song="song"></MusicCard>
      </div>
    </div>
  <Player :currentSong="this.currentSong"></Player>
  </div>
</template>

<script>
import Loader from '@/components/Loader'
import NavBar from '@/components/NavBar'
import SideBar from '@/components/SideBar'
import Player from '@/components/Player'
import MusicCard from '@/components/MusicCard';
export default {
    components:{
        Loader,
        MusicCard,
        SideBar,
        NavBar,
        Player
    },
    methods:{
        playSong (song) {
          this.currentSong = song;
        }
    },
    data(){
        return{
            currentSong : '',
            songs:[
                {name:'Artist',
                artist:'artist',
                path: 'music.mp3'},
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
@media only screen and (max-width: 600px) {
  .song__holder {
    grid-template-columns: 1fr;
  }
}
</style>