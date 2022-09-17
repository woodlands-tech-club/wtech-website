<script>
	import '../app.css';
	import Navbar from '../components/Navbar.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<main class="lg:mx-[20%] mx-[10%]">
	<Navbar />

	<slot />

	<Footer />
</main>
