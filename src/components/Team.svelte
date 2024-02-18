<script lang="ts">
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';

	let members = [
		["Marko Mihajlović", "kombinuje fiziku i mehatroniku, oblikujući mehaničko srce našeg robota sa preciznošću.", "/mihajlovic.jpg"],
		["Mihailo Pešić", "je vezni član, spajajući fiziku i programiranje s veštinama u komunikaciji, držeći tim u sinergiji.", "/pesic.jpg"],
		["Aleksa Bolić", "donosi kreativne iskre u programiranju i fizici, osmišljavajući inovacije koje vode tim napred.", "/bolic.jpg"],
		["Vukašin Rondović", "je majstor modelovanja, pretvarajući ideje u konkretne, funkcionalne delove robota.", "/rondovic.jpg"],
		["Aleksa Ognjanović", "je naš softverski guru, sa izvanrednim veštinama u programiranju i matematici, ključan za robota koji razmišlja brzo.", "/ognjanovic.jpg"],
		["Kosta Jovanović", "", "/jovanovic.jpg"],
	];
</script>


<div class="bg-base-100 w-full py-8" id="team">
	<div class="container mx-auto px-2">
		<h3 class="text-4xl font-bold text-center">Tim</h3>
		<div class="lg:grid justify-center grid-cols-[repeat(auto-fit,minmax(min-content,450px))] flex flex-col">
			{#each members as member }
				<div class="card shadow-lg m-4">
					<figure>
						<img
							src="{member[2]}"
							class="aspect-square object-cover object-top"
							alt="{member[0]} slika"
						/>
					</figure>
					<div class="card-body">
						<p class="card-title self-center">{member[0]}</p>
						<p class="text-center">{member[1]}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>
