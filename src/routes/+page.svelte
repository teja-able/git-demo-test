<script>
	import CountriesData from '$lib/components/CountriesData.svelte';
	import GradientButton from '../lib/components/GradientButton.svelte';
  let selectedOption = '';
</script>

<main class="flex flex-col justify-center main bg-black text-white h-screen">
	<CountriesData />
	<h1 class="text-[110px] text-center">HELLO world</h1>
	<CountriesData />
	<div class="flex items-center gap-10 justify-center mt-40">
		<GradientButton />
      <div class="p-4">
        <label class="block mb-2 font-bold">Choose one  :</label>
        <label class="inline-flex items-center">
          <input type="radio" bind:group={selectedOption} value="yes" />
          <span class="ml-2">Yes</span>
        </label>
        
        <label class="inline-flex items-center ml-4">
          <input type="radio" bind:group={selectedOption} value="no" />
          <span class="ml-2">No</span>
        </label>
        
        <p class="mt-4">Selected: {selectedOption}</p>
      </div></div>

	
</main>
