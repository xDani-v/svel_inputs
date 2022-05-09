<script>
	let rango = "";
	let check = false;
	let frutas = ['limon','frutilla','tomate'];
	let array = []
	let radio = "";
	$: console.log(array);
</script>

<div>
	{#each frutas as fruta}
		 <input type="checkbox" value={fruta} bind:group={array}>
		 {fruta}
	{/each}
	<p>fruta:{array}</p>

	<!-- {#each frutas as fruta}
		 <input type="radio" value={fruta} bind:group={radio}>
		 {fruta}
	{/each}
	<p>fruta:{radio}</p> -->


	<!-- <h1>Buildings</h1>

	<input type="checkbox" bind:checked={check}>
	<p>{check}</p> -->
	<!-- <input type="range" bind:value={rango} min="0" max="100">
	<p>texto:{rango}</p> -->
</div>
