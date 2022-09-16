<div class="flex justify-between my-3 items-center md:flex-row lg:flex-row flex-col">
	<a href="/">
		<div class="flex gap-3 items-center">
			<img src="gear_logo_colored.png" alt="logo" class="h-14 w-14" />
			<div class="text-2xl font-bold">Woodlands Tech Club</div>
		</div>
	</a>

	<h5>📍 Mississauga, ON</h5>
	<!-- <ul class="flex gap-5">
		<li>
			<a href="/">Home</a>
		</li>
		<li>
			<a href="/about">About</a>
		</li>
		<li>
			<a href="/contact">Contact</a>
		</li>
	</ul> -->
</div>

<hr />

<style>
	.spinning-logo {
		-webkit-animation: spin 10s linear infinite;
		-moz-animation: spin 10s linear infinite;
		animation: spin 10s linear infinite;
	}
	@-moz-keyframes spin {
		50% {
			-moz-transform: rotate(90deg);
		}
		100% {
			-moz-transform: rotate(360deg);
		}
	}
	@-webkit-keyframes spin {
		100% {
			-webkit-transform: rotate(360deg);
		}
	}

	@keyframes spin {
		100% {
			-webkit-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}
</style>
