<script lang="ts">
	import AboutUs from "$components/AboutUs.svelte";
	import Contact from "$components/Contact.svelte";
	import Drawer from "$components/Drawer.svelte";
	import Footer from "$components/Footer.svelte";
	import Gallery from "$components/Gallery.svelte";
	import Hero from "$components/Hero.svelte";
    import Navbar from "$components/Navbar.svelte";
	import Sponsors from "$components/Sponsors.svelte";
	import Team from "$components/Team.svelte";
</script>

<div class="drawer pt-16">
	<input id="drawer-checkbox" type="checkbox" class="drawer-toggle" />
	<div class="drawer-side z-50">
		<label for="drawer-checkbox" class="drawer-overlay" />
		<Drawer />
	</div>
	<main class="drawer-content">
		<Navbar />

		<Hero />

		<AboutUs />

		<Team />

		<Sponsors />

		<!-- <Gallery /> -->

		<Contact />

		<Footer />
	</main>
</div>
