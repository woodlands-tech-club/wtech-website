<script>
	export let discord_link;
	export let instagram_link;
	export let github_link;
</script>

<div class="flex flex-col md:flex-row items-center gap-5 my-10">
	<div class="md:w-[50%]">
		<p class="font-semibold mb-2 text-xl">
			The Woodlands Tech Club is a school club of the Woodlands Public School in Mississauga, ON.
		</p>

		<p class="font-normal text-md">
			We are a group of students who are passionate about technological education. We strive to
			promote tech literacy and make it accessible to everyone.
		</p>

		<div class="mt-6 flex gap-5">
			<a href={discord_link}>
				<img src="/discord.svg" alt="discord" class="h-9 blue-500" />
			</a>
			<a href={instagram_link}>
				<img src="/instagram.svg" alt="instagram" class="h-9 blue-500" />
			</a>
			<a href={github_link}>
				<img src="/github.svg" alt="github" class="h-9 blue-500" />
			</a>
		</div>
	</div>
	<img src="students.jpg" alt="group photo" class="md:w-[50%] md:h-auto shadow-md rounded-md" />
</div>
