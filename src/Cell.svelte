<script>
	export let active = false;

	const toggleActive = () => {
		active = !active;
	}
</script>

<style>

	td {
		padding-top: 0.15em;
		padding-bottom: 0.15em;
		padding-left: 0.1em;
		padding-right: 0.1em;
	}
	
	div {
		background: #444;
		border-radius: 3px;
		width: 1.5em;
		height: 1.5em;
		transition: 0.1s ease-in;
	}

	div.active {
		background: #fff;
		box-shadow: 0px 0px 8px 2px rgb(255, 255, 255, 0.5);
	}

</style>

<td>
	<div class:active={active} on:click={toggleActive}>
	</div>
</td>