<script>
	import { Trash2 } from 'lucide-svelte';

	let { name, image, price } = $props();
</script>

<div class="flex items-center justify-between bg-slate-300 p-5">
	<div class="flex items-center gap-3">
		<img src={image} alt="" class=" size-28 object-cover" />
		<div>
			<h3 class="text-xl font-bold">{name}</h3>
			<h3 class="mt-1 text-lg">{price}грн</h3>
		</div>
	</div>
	<button class="p-2 hover:bg-slate-400"><Trash2 /></button>
</div>
