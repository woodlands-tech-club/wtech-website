<script>
	export let title;
	export let subtitle;
	export let gradient;
	export let article_link;
</script>

<a
	href={article_link}
	class="min-h-[200px] text-white flex flex-col bg-gradient-to-b {gradient} rounded-md"
>
	<div class="mt-auto p-4">
		<h3 class="text-lg font-semibold leading-tight mb-2">{title}</h3>
		<p class="text-sm">{subtitle}</p>
	</div>
</a>

<style>
</style>
