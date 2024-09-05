<script>
	import CountriesData from '$lib/components/CountriesData.svelte';
	import GradientButton from '../lib/components/GradientButton.svelte';
</script>

<main class="flex flex-col justify-center main bg-black text-white h-screen">
	<CountriesData />
	<h1 class="text-[110px] text-center">HELLO world</h1>
	<CountriesData />
	<div class="flex items-center gap-10 justify-center mt-40">
		<GradientButton />
		<p>click here</p>
		<GradientButton />
	</div>
</main>
