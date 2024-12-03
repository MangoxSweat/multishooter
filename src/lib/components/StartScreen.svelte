<script>
	import { createEventDispatcher } from 'svelte';

	const dispatch = createEventDispatcher();

	function startGame() {
		dispatch('start');
	}
</script>

<h1>Multiplayer first person shooter</h1>
<button on:click={startGame}>Start</button>

<style>
	body {
		font-family: 'Press Start 2P', cursive;
		background-color: black;
		color: green;
		text-align: center;
		margin: 0;
		display: flex;
		flex-direction: column;
		justify-content: center;
		height: 100vh;
	}
	button {
		font-family: 'Press Start 2P', cursive;
		background-color: black;
		color: green;
		border: 2px solid green;
		padding: 10px 20px;
		cursor: pointer;
	}
	button:hover {
		background-color: green;
		color: black;
	}
</style>
