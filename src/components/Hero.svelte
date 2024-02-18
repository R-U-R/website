<script lang="ts">
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
</script>

<div class="w-screen h-[80vh] relative">
	<div class="absolute top-1/2 left-1/2 z-10 -translate-x-1/2 -translate-y-1/2 space-y-4 text-center">
		<h1 class="font-bold text-4xl">Mi smo R.U.R.</h1>
		<p class="font-semibold text-lg">Tim za medjunarodno takmičenje iz robotike - Eurobot.</p>
		<a class="btn btn-neutral text-lg" href="#aboutus">Saznaj više</a>
	</div>
	<Splide
		aria-label="My Favorite Images"
		options={{
			type: 'loop',
			autoplay: true,
			pauseOnHover: true,
			cover: true,
			width: "100vw",
			height: "80vh",
		}}
	>
		<SplideSlide>
			<img class="-z-50" src="https://picsum.photos/1920/1080" alt="1" />
		</SplideSlide>
		<SplideSlide>
			<img class="-z-50" src="https://picsum.photos/1920/1080" alt="2" />
		</SplideSlide>
		<SplideSlide>
			<img class="-z-50" src="https://picsum.photos/1920/1080" alt="3" />
		</SplideSlide>
		<SplideSlide>
			<img class="-z-50" src="https://picsum.photos/1920/1080" alt="4" />
		</SplideSlide>
	</Splide>
</div>
