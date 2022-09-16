<script>
	import Article from './Article.svelte';
</script>

<div class="flex items-center gap-3">
	<h2 class="text-2xl font-semibold">✒️ Blog</h2>
	<h4 class="underline"><a href="/blog">View all</a></h4>
</div>
<hr />

<ul class="mt-4 flex w-[100%] gap-4 justify-between flex-col md:flex-row mb-14">
	<li class="w-[100%] lg:max-w-[30%]">
		<Article
			title="Intro to the woodlands tech club"
			subtitle="An introductory blog to wtech's internal organization"
			gradient="from-cyan-200 to-blue-400"
			article_link="/intro"
		/>
	</li>
	<li class="w-[100%] lg:max-w-[30%]">
		<Article
			title="Coming Soon..."
			subtitle="This article has not been written yet"
			gradient="from-gray-200 to-gray-400"
			article_link="#"
		/>
	</li>
	<li class="w-[100%] lg:max-w-[30%]">
		<Article
			title="Coming Soon..."
			subtitle="This article has not been written yet"
			gradient="from-gray-200 to-gray-400"
			article_link="#"
		/>
	</li>
</ul>
