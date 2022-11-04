<script>
	export let discord_link;
	export let instagram_link;
	export let github_link;
</script>


<section class="text-white ml-[10%] mt-32 relative">
	<!-- <img src="gear_logo_colored.svg" alt="group photo" class="absolute h-[100vh] top-[40px] right-[-100px]" /> -->

			<img src="/gear_logo_new.png" class="absolute sm:w-[200px] w-[120px] z-[-100]  sm:left-[-5rem] left-[-2rem] top-[-1rem]">
			<div class="">
				<h1 class="mb-16 text-7xl sm:text-9xl ps150 tracking-tight rotate-[-2deg] max-w-[90%]">
					<span class="pl-8">The</span><br><span class="">Woodlands</span><br><span class="pl-12">Tech Club</span>
					<!-- The <span class="highlight font-normal ps150"></span> is a school club of the
					Woodlands Secondary School in Mississauga, ON. -->
				</h1>

				<p class="sm:text-2xl text-lg as130 sm:max-w-2xl pr-3 text-pink-500">
					3D printing, consumer technology, tech literacy
				</p>

				<!-- <div class="mt-10 flex gap-5">
					<a href={discord_link}>
						<img src="/discord.svg" alt="discord" class="h-9" />
					</a>
					<a href={instagram_link}>
						<img src="/instagram.svg" alt="instagram" class="h-9" />
					</a>
					<a href={github_link}>
						<img src="/github.svg" alt="github" class="h-9 " />
					</a>
				</div> -->
			</div>
			
		
		<!-- <div class="custom-shape-divider-bottom-1664676304">
			<svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
				<path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
			</svg>
		</div> -->

</section>

<style>
	/* .bg-image {
		background: url('students.jpg');
		background-attachment: fixed;
		background-position: right;
		background-position-x: 400px;
		background-size: cover;
	} */
	.bg-lines {
		background: linear-gradient(-90deg, rgba(255, 255, 255, 10) 20%, rgba(255, 255, 255, 10) 75%);
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
	.custom-shape-divider-bottom-1664676304 {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.custom-shape-divider-bottom-1664676304 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 106px;
    transform: rotateY(180deg);
}

.custom-shape-divider-bottom-1664676304 .shape-fill {
    fill: #FFFFFF;
}


</style>
