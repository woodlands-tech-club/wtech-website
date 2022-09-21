<script>
	export let discord_link;
	export let instagram_link;
	export let github_link;
</script>

<section class="bg-image overflow-hidden relative">
	<!-- <img src="gear_logo_colored.svg" alt="group photo" class="absolute h-[100vh] top-[40px] right-[-100px]" /> -->

	<div class="bg-lines">
		<div class="flex flex-col md:flex-row items-center gap-5 h-[100vh] max-w-screen-xl m-auto ">
			<div class="md:w-[50%] z-10">
				<div class="font-light mb-12 text-4xl">
					The <span class="highlight font-normal">Woodlands Tech Club</span> is a school club of the
					Woodlands Secondary School in Mississauga, ON.
				</div>

				<p class="font-normal text-gray-700 text-lg">
					We are a group of students who are passionate about technological education. We strive to
					promote tech literacy and make it accessible to everyone.
				</p>

				<div class="mt-10 flex gap-5">
					<a href={discord_link}>
						<img src="/discord.svg" alt="discord" class="h-9" />
					</a>
					<a href={instagram_link}>
						<img src="/instagram.svg" alt="instagram" class="h-9" />
					</a>
					<a href={github_link}>
						<img src="/github.svg" alt="github" class="h-9 " />
					</a>
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	.bg-image {
		background: url('students.jpg');
		background-attachment: fixed;
		background-position: right;
		background-position-x: 400px;
		background-size: cover;
	}
	.bg-lines {
		background: linear-gradient(-90deg, rgba(255, 255, 255, 0.2) 20%, rgb(217, 223, 227) 75%);
		/* linear-gradient(180deg, rgba(255,255,255,0) 60%, rgba(255, 255, 255, 0.5) 100%),
		/* linear-gradient(41deg, rgba(255,255,255,0) 21%, rgb(191, 228, 248) 34%, rgba(255,255,255,0) 44%), 
		linear-gradient(41deg, rgba(255,255,255,0) 21%, rgba(64, 140, 181, 0.3) 34%, rgba(255,255,255,0) 44%), */
	}
	.highlight {
		position: relative;
	}
	.highlight::before {
		background: rgb(105, 177, 222);
		background: linear-gradient(292deg, rgba(105, 177, 222, 1) 0%, rgba(149, 189, 255, 1) 100%);
		content: '';
		position: absolute;
		width: calc(100%);
		height: 75%;

		bottom: 0;
		z-index: -1;
		transform: rotate(-1.5deg);
	}
</style>
