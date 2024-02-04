<script>
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
</script>

<div class="w-full py-8 bg-base-100" id="gallery">
	<div class="mx-auto container">
		<h1 class="text-4xl text-center font-bold">Galerija</h1>

		<div class="m-8 shadow-lg p-4 rounded-box bg-base-100">
			<Splide
				options={{
					perPage: 3,
					perMove: 1,
					heightRatio: 0.2,
					cover: true,
					trimSpace: false,
					gap: '1em',
					breakpoints: {
						1024: {
							padding: '2rem',
							perPage: 1,
							heightRatio: 0.4
						}
					}
				}}
			>
				{#each { length: 15 } as _, i}
					<SplideSlide>
                        <img src="https://picsum.photos/1920/1080" alt="" />
					</SplideSlide>
				{/each}
			</Splide>
		</div>
	</div>
</div>
