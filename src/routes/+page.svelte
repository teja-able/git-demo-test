<script>
	import GradientButton from '../lib/components/GradientButton.svelte';
  let selectedOption = '';
</script>

<main>
	<h1 class="text-[110px] text-center bg-gray-100">HELLO world</h1>
	<div class="flex items-center justify-center h-screen bg-gray-100">
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

		<div>click here <GradientButton />
	</div>
</main>
