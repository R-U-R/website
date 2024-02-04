<script>
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
</script>

<div class="bg-base-100 w-full py-8">
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
		{#each { length: 15 } as _, i}
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
						<p class="card-title self-center">Ime Prezime</p>
						<p>
							Lorem ipsum dolor sit amet consectetur, adipisicing elit. Blanditiis totam asperiores
							nesciunt, doloribus ipsa ipsam assumenda laudantium libero nemo expedita culpa
							necessitatibus eveniet consequuntur unde repudiandae itaque voluptate possimus.
							Commodi?
						</p>
					</div>
				</div>
			</SplideSlide>
		{/each}
	</Splide>
</div>
