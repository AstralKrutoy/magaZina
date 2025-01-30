<script>
	import Header from '$lib/comps/Header.svelte';
	import CategoryItem from '$lib/comps/CategoryItem.svelte';
	let category = [
		{
			id: 1,
			name: 'Electronics',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 2,
			name: 'Fashion',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 3,
			name: 'Home Appliances',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 4,
			name: 'Books',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 5,
			name: 'Toys',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 6,
			name: 'Sports',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 7,
			name: 'Beauty',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 8,
			name: 'Health',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 9,
			name: 'Grocery',
			img: 'https://placehold.co/600x400/EEE/31343C'
		},
		{
			id: 10,
			name: 'Automotive',
			img: 'https://placehold.co/600x400/EEE/31343C'
		}
	];
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
