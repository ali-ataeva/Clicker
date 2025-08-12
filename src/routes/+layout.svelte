<script lang="ts">
	import '../app.css';

	let clickCount = $state(0);

	function SimpleAdd() {
		clickCount += 1;
	}
	function Reset() {
		clickCount = 0;
	}
</script>

<main>
	<button class="clickButton" onclick={SimpleAdd}>
		<p>Click here!</p>
	</button>
	<p>Your click count {clickCount}</p>
	<button class="resetButton" onclick={Reset}>
		<p>Reset clicks</p>
	</button>
</main>

<style>
	.clickButton {
		background-color: rgb(187, 136, 234);
		box-shadow: inset rgba(0, 0, 0, 0.435) -2px -2px 2px 2px;
		width: 200px;
		height: 200px;
		border-radius: 100px;
	}
	.resetButton {
		background-color: red;
		padding: 10px 20px;
		border-radius: 10px;
		box-shadow: inset rgba(0, 0, 0, 0.269) -2px -2px 2px 2px;
	}
	main {
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		gap: 20px;
	}
</style>
