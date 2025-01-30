<script>
	import Header from '$lib/comps/Header.svelte';
	import ProductItem from '../lib/comps/ProductItem.svelte';
	let tovar = [
		{
			id: 1,
			name: 'unitaz',
			price: 263,
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 2,
			name: 'mashina',
			price: 789,
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 3,
			name: 'dom',
			price: 2125663,
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 4,
			name: 'telephon',
			price: 896,
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 5,
			name: 'knizhka',
			price: 89,
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 6,
			name: 'router',
			price: 233,
			img: 'https://placehold.co/600x400/EEE/31343C'
		}
	];
</script>

<Header />

<main class="container">
	<h2>Популярні товари</h2>
	<div class="grid grid-cols-4 gap-6">
		{#each tovar as item}
			<ProductItem name={item.name} price={item.price} image={item.img} />
		{/each}
	</div>
</main>
