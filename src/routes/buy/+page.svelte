<script>
	import Header from '$lib/comps/Header.svelte';
	import CartItem from '$lib/comps/CartItem.svelte';
	import { products } from '../../lib/db';

	let mylist = [1, 8, 4];
</script>

<Header />
<main class="container mt-10">
	<div class="mb-4 flex items-center justify-between">
		<h2 class="mb-1 mt-4 text-xl">Кошик</h2>
		<button class="bg bg-slate-300 p-2 px-6 font-bold hover:bg-slate-400"
			>Оформити замовлення</button
		>
	</div>
	<div class="flex flex-col gap-5">
		{#each products as item}
			{#if item.id in mylist}
				<CartItem name={item.name} image={item.img} price={item.price} />
			{/if}
		{/each}
	</div>
</main>
