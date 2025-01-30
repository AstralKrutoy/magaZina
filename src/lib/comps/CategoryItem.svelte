<script>
	let { name, image } = $props();
</script>

<a href="/">
	<div class="bg-slate-300">
		<img src={image} alt="" />
		<div class="flex items-center justify-center px-4 py-2">
			<p class="ml-3 font-bold">{name}</p>
		</div>
	</div>
</a>
