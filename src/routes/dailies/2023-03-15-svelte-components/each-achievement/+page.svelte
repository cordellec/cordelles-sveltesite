<script>
	const todoList = [
		'Get out of bed',
		'Make coffee',
		'Read feeds',
		'Have shower',
		'Brush teeth',
		'Get dressed',
		'Leave for work',
		'Get breakfast to go'
	];
</script>

<div class="container">
<main>
<h1>Each Loop Svelte</h1>

<ol>
	{#each todoList as items}
		<li>{items}</li>
	{/each}
</ol>
</main>
</div>


<style>
.container {
	display: flex;
	flex-direction: column;
	justify-content:center;
	align-items: center;
	flex-grow: 1;
}
</style>