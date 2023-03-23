<script>
	import { todoList } from './todoList.js';
</script>

<main>
	<h1>Each Loop Svelte</h1>

	<ol>
		{#each todoList as items}
			<li>{items}</li>
		{/each}
	</ol>
</main>