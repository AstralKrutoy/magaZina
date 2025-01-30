<script>
	import Header from '$lib/comps/Header.svelte';
	import CategoryItem from '$lib/comps/CategoryItem.svelte';
	import { category } from '../../lib/db.js';
</script>

<Header />

<main class="container">
	<h2 class="mb-1 mt-4 text-xl">Категорії</h2>
	<div class="grid grid-cols-4 gap-6">
		{#each category as categ}
			<CategoryItem name={categ.name} image={categ.img} />
		{/each}
	</div>
</main>
