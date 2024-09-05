<script>
	// Any button-related logic can go here if necessary
</script>

<button class="gradient-btn bg-gradient-to-r from-purple-400 via-pink-500 to-red-500 text-white">
	hover the button
</button>

<style>
	/* Custom hover animation */
	.gradient-btn {
		position: relative;
		padding: 16px 32px;
		font-size: 18px;
		font-weight: bold;
		border-radius: 8px;
		transition:
			transform 0.3s ease,
			box-shadow 0.3s ease;
		overflow: hidden;
	}

	.gradient-btn:hover {
		transform: scale(1.1);
		box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
	}

	.gradient-btn::before {
		content: '';
		position: absolute;
		top: 50%;
		left: 50%;
		width: 300%;
		height: 300%;
		background: rgba(255, 255, 255, 0.2);
		transform: translate(-50%, -50%) scale(0);
		border-radius: 50%;
		transition: transform 0.6s ease;
	}

	.gradient-btn:hover::before {
		transform: translate(-50%, -50%) scale(1);
	}
</style>
