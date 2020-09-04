<template>
	<div class="player flex items-center justify-center bg-red-lightest">
		<div class="player__box p-2 m-2 text-gray-700 bg-gray-900 rounded-lg shadow-lg">
			<div class="flex player_inner">
				<div>
					<img class="player__album rounded hidden md:block" src="../storage/images/logo_transparent.png" alt="Album Pic">
				</div>
				<div class="w-full p-2">
					<div class="flex justify-between">
						<div>
							<h3 class="text-grey-darkest font-medium">A Sky Full of Stars</h3>
							<p class="text-sm text-grey mt-1">Ghost Stories</p>
						</div>
					</div>
					<div class="player__actions flex justify-between items-center mt-2">
						<div class="text-grey-darker">
							<svg class="w-4 h-4" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M6.59 12.83L4.4 15c-.58.58-1.59 1-2.4 1H0v-2h2c.29 0 .8-.2 1-.41l2.17-2.18 1.42 1.42zM16 4V1l4 4-4 4V6h-2c-.29 0-.8.2-1 .41l-2.17 2.18L9.4 7.17 11.6 5c.58-.58 1.59-1 2.41-1h2zm0 10v-3l4 4-4 4v-3h-2c-.82 0-1.83-.42-2.41-1l-8.6-8.59C2.8 6.21 2.3 6 2 6H0V4h2c.82 0 1.83.42 2.41 1l8.6 8.59c.2.2.7.41.99.41h2z"/></svg>
						</div>
						<div class="text-grey-darker">
							<svg class="w-4 h-4" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M4 5h3v10H4V5zm12 0v10l-9-5 9-5z"/></svg>
						</div>
						<div class="text-white p-3 rounded-full bg-red-light shadow-lg">
							<svg class="w-4 h-4" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M5 4h3v12H5V4zm7 0h3v12h-3V4z"/></svg>
						</div>
						<div class="text-grey-darker">
							<svg class="w-4 h-4" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M13 5h3v10h-3V5zM4 5l9 5-9 5V5z"/></svg>
						</div>
						<div class="text-grey-darker">
							<svg class="w-4 h-4" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M5 4a2 2 0 0 0-2 2v6H0l4 4 4-4H5V6h7l2-2H5zm10 4h-3l4-4 4 4h-3v6a2 2 0 0 1-2 2H6l2-2h7V8z"/></svg>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {

}
</script>

<style>
.player{
    width:100%;
    max-height: 150px;
    position: sticky;
    bottom: 0;
}
.player_inner{
    max-height: 150px;
}
.player__box{
    width: 100%;
}
.player__album{
    width:200px;
    display: flex;
    justify-content: center;
    height: 100%;
    object-fit: cover;
}
.player__actions{
    width:250px;
    margin-left: 1rem;
}
@media only screen and (max-width: 600px) {
	.player__album{
		display: none;
	}
}
</style>