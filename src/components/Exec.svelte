<script>
	export let exec_name;
	export let exec_role;
	export let exec_img;
</script>

<div class="text-center m-auto mt-4">
	<img src={exec_img} alt={exec_name} class="w-32 h-32 shadow-md mb-5 rounded-md" />
	<h3 class="text-lg font-medium">{exec_name}</h3>
	<h4 class="text-blue-400">— {exec_role}</h4>
</div>
