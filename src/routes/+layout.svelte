<script lang="ts">
	import '../app.css';

	let clickCount = $state(0);

	function Add() {
		clickCount += 1;
	}
</script>

<main>
	<button onclick={Add}>
		<p>click here</p>
	</button>

	<p>Your click count {clickCount}</p>
</main>
