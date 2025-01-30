<script>
	import Header from '$lib/comps/Header.svelte';
	import ProductItem from '../lib/comps/ProductItem.svelte';
	import { tovar } from '../lib/db.js';
</script>

<Header />

<main class="container">
	<h2 class="mb-1 mt-4 text-xl">Популярні товари</h2>
	<div class="grid grid-cols-4 gap-6">
		{#each tovar as item}
			<ProductItem name={item.name} price={item.price} image={item.img} />
		{/each}
	</div>
</main>
