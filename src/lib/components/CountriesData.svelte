<script>
	const countryData = [
		{ name: 'India', pincode: '110001', flag: '🇮🇳' },
		{ name: 'United States', pincode: '10001', flag: '🇺🇸' },
		{ name: 'United Kingdom', pincode: 'SW1A 1AA', flag: '🇬🇧' },
		{ name: 'Canada', pincode: 'M5H 2N2', flag: '🇨🇦' },
		{ name: 'Australia', pincode: '2000', flag: '🇦🇺' },
		{ name: 'Germany', pincode: '10115', flag: '🇩🇪' },
		{ name: 'France', pincode: '75001', flag: '🇫🇷' },
		{ name: 'Japan', pincode: '100-0001', flag: '🇯🇵' },
		{ name: 'China', pincode: '100000', flag: '🇨🇳' },
		{ name: 'Brazil', pincode: '01000-000', flag: '🇧🇷' },
		{ name: 'South Africa', pincode: '0002', flag: '🇿🇦' },
		{ name: 'Russia', pincode: '101000', flag: '🇷🇺' },
		{ name: 'Italy', pincode: '00100', flag: '🇮🇹' },
		{ name: 'Mexico', pincode: '01000', flag: '🇲🇽' },
		{ name: 'Argentina', pincode: 'C1001AAG', flag: '🇦🇷' },
		{ name: 'South Korea', pincode: '03000', flag: '🇰🇷' }
	];
</script>

<div class="marquee">
	<ul class="marquee-content flex gap-8">
		{#each countryData as country}
			<li class="flex items-center gap-2 w-50">
				{country.flag}
				{country.name} - Pincode: {country.pincode}
			</li>
		{/each}
	</ul>
	<ul class="marquee-content flex gap-8">
		{#each countryData as country}
			<li class="flex items-center gap-2 w-50">
				{country.flag}
				{country.name} - Pincode: {country.pincode}
			</li>
		{/each}
	</ul>
</div>

<style>
	.marquee {
		white-space: nowrap;
		overflow: hidden;
		display: flex;
		align-items: center;
	}

	.marquee-content {
		/* display: inline-block; */
		white-space: nowrap;
		animation: marquee 40s linear infinite;
	}

	@keyframes marquee {
		100% {
			transform: translateX(100%);
		}
		100% {
			transform: translateX(-100%);
		}
	}
</style>
