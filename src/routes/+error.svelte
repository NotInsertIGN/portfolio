<script lang="ts">
	import { page } from "$app/stores";
</script>

<h1>
	<span style="color: crimson">ERROR {$page.status}</span><br>{$page.error.message}
</h1>
<h1>
	<a href="/">Return to Home</a>
</h1>

<style>
	h1 {
			color: #cdddff;
	}
</style>