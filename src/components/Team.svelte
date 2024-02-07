<script lang="ts">
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';

	let members = [
		["Aleksa Ognjanović", "je naš softverski guru, sa izvanrednim veštinama u programiranju i matematici, ključan za robota koji razmišlja brzo."],
		["Marko Mihajlović", "kombinuje fiziku i mehatroniku, oblikujući mehaničko srce našeg robota sa preciznošću."],
		["Mihailo Pešić", "je vezni član, spajajući fiziku i programiranje s veštinama u komunikaciji, držeći tim u sinergiji."],
		["Aleksa Bolić", "donosi kreativne iskre u programiranju i fizici, osmišljavajući inovacije koje vode tim napred."],
		["Vukašin Rondović", "je majstor modelovanja, pretvarajući ideje u konkretne, funkcionalne delove robota."],
	];
</script>

<div class="bg-base-100 w-full py-8" id="team">
	<h3 class="text-4xl font-bold text-center">Tim</h3>

	<Splide
		options={{
			type: 'loop',
			autoplay: true,
			pauseOnHover: true,
			focus: 'center',
			perPage: 7,
			padding: '5rem',
			pagination: false,
			breakpoints: {
				2700: {
					perPage: 6
				},
                2400: {
					perPage: 5
				},
                2000: {
                    perPage: 4
                },
                1700: {
                    perPage: 3
                },
                1400: {
                    perPage: 2
                },
                800: {
                    perPage: 1
                },
			}
		}}
	>
		{#each members as member }
			<SplideSlide>
				<div class="card shadow-lg m-4">
					<figure>
						<img
							src="https://picsum.photos/1920/1080"
							class="aspect-square object-cover"
							alt="Shoes"
						/>
					</figure>
					<div class="card-body">
						<p class="card-title self-center">{member[0]}</p>
						<p>{member[1]}</p>
					</div>
				</div>
			</SplideSlide>
		{/each}
	</Splide>
</div>
