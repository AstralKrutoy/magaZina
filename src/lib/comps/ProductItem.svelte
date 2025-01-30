<script>
	import { Heart } from 'lucide-svelte';

	let { name, price, image } = $props();
</script>

<!-- <p>{name} - {price}</p> -->

<div class="bg-slate-300">
	<img src={image} alt="" />
	<div class="flex items-center justify-between px-4 py-2">
		<p class="ml-3 font-bold">{name}</p>
		<p>{price}$</p>
	</div>
	<div class="flex justify-between gap-4 rounded border px-4 px-6 py-2 py-6 text-black shadow">
		<button class="w-full rounded bg-white px-7 py-1">Додати в кошик</button>
		<button class="rounded bg-white px-3 px-4 py-1">
			<Heart />
		</button>
	</div>
</div>
