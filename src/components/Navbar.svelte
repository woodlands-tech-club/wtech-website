<nav class="absolute w-[100%] shadow-lg bg-gray-800 z-10">
	<div
		class="flex justify-between  items-center md:flex-row lg:flex-row flex-col max-w-screen-xl m-auto"
	>
		<a href="/">
			<div class="flex gap-3 items-center">
				<img src="wtech_white.png" alt="logo" class="h-14 w-auto" />
				<!-- <div class="text-xl font-semibold text-white font-[source_code_pro]">Woodlands Tech Club</div> -->
			</div>
		</a>

		<!-- <h5>📍 Mississauga, ON</h5> -->
		<ul class="flex gap-16 text-white font-[Source_Code_Pro] items-center ">
			<li>
				<a href="/" class="h-28 px-4 flex items-center nav-button">Home</a>
			</li>
			<li>
				<a href="/about" class="h-28 px-4 flex items-center nav-button">About</a>
			</li>
			<li>
				<a href="/contact" class="h-28 px-4 flex items-center nav-button">Contact</a>
			</li>
		</ul>
	</div>
</nav>

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

	.nav-button {
		box-shadow: rgba(219, 219, 219, 0.495) 0px -30px 20px -28px inset;
		transition: ease 0.3s;
	}

	.nav-button:hover {
		box-shadow: rgba(219, 219, 219, 0.495) 0px -40px 20px -28px inset;
	}
</style>
