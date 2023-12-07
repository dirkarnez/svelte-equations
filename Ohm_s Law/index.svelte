<script>
	$: i = 1;
	$: r = 1;

	// the `$:` means 're-run whenever these values change'
	$: v = i * r;


	function handleClickI() {
		i += 1;
	}

	function handleClickR() {
		r += 1;
	}
</script>

<button on:click={handleClickI}>
	Count: {v} = {i} * {r}
</button>

<button on:click={handleClickR}>
	Count: {v} = {i} * {r}
</button>

