<script lang="ts">
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
</script>

<Splide
	aria-label="My Favorite Images"
	options={{
		type: 'loop',
		autoplay: true,
		pauseOnHover: true,
		cover: true,
		height: '80vh',
		width: '100vw',
	}}
>
	<SplideSlide>
		<img class="-z-50" src="https://picsum.photos/1920/1080" alt="Image 1" />
	</SplideSlide>
	<SplideSlide>
		<img class="-z-50" src="https://picsum.photos/1920/1080" alt="Image 2" />
	</SplideSlide>
	<SplideSlide>
		<img class="-z-50" src="https://picsum.photos/1920/1080" alt="Image 2" />
	</SplideSlide>
	<SplideSlide>
		<img class="-z-50" src="https://picsum.photos/1920/1080" alt="Image 2" />
	</SplideSlide>
</Splide>
