<script lang="ts">
	import { spring } from 'svelte/motion';
	let count = 0;
</script>

<div class="counter">
	<button on:click={() => (count -= 1)} aria-label="Decrease the counter by one">
		-
	</button>
	<div>
			<strong>{Math.floor(count)}</strong>
	</div>
	<button on:click={() => (count += 1)} aria-label="Increase the counter by one">
		+
	</button>
</div>

