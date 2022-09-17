<script>
	import Hero from '../components/Hero.svelte';
	import WhatWeDo from '../components/WhatWeDo.svelte';
	import Blog from '../components/Blog.svelte';
	import Team from '../components/Team.svelte';

	let discord_link = 'https://discord.gg/3s4DYcbJ37';
	let instagram_link = 'https://www.instagram.com/woodlands.tech/';
	let github_link = 'https://github.com/woodlands-tech-club';
</script>

<Hero {discord_link} {instagram_link} {github_link} />
<Blog />
<WhatWeDo />
<Team />
