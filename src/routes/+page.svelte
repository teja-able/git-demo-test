<script>
	import CountriesData from '$lib/components/CountriesData.svelte';
	import GradientButton from '../lib/components/GradientButton.svelte';
	let selectedOption = '';
</script>

<main class="flex flex-col justify-center main bg-black text-white h-screen">
	<CountriesData />
	<h1 class="text-[110px] text-center">HELLO World</h1>
	<CountriesData />
	<div class="flex items-center gap-10 justify-center mt-40">
		<GradientButton />
		<div class="p-4">
			<label class="block mb-2 font-bold">Choose one :</label>
			<label class="inline-flex items-center">
				<input type="radio" bind:group={selectedOption} value="yes" />
				<span class="ml-2">Yes</span>
			</label>

			<label class="inline-flex items-center ml-4">
				<input type="radio" bind:group={selectedOption} value="no" />
				<span class="ml-2">No</span>
			</label>

			<p class="mt-4">Selected: {selectedOption}</p>
		</div>
	</div>
	<h3
		class="text-5xl text-center mt-12 bg-transparent bg-gradient-to-r from-purple-400 via-pink-500 to-red-500 from-green-700 border-4 via-blue-500 to-red-500 text-transparent bg-clip-text max-w-max mx-auto"
	>
		OPTIMUS PRIME
	</h3>
</main>
