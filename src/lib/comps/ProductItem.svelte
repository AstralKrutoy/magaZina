<script>
	import { Heart } from 'lucide-svelte';

	let { name, price, image } = $props();
</script>

<!-- <p>{name} - {price}</p> -->

<div class="bg-slate-300">
	<img src={image} alt="" />
	<div class="flex items-center justify-between px-4 py-2">
		<p class="font-bold">{name}</p>
		<p>{price}$</p>
	</div>
	<div class="flex justify-between rounded border px-4 px-6 py-2 py-6 text-black shadow">
		<button class="rounded bg-white px-3 py-1">Додати в кошик</button>
		<button>
			<Heart />
		</button>
	</div>
</div>
