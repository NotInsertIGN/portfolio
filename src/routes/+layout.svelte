<script lang="ts">
	import "../app.css";
	import "../nprogress.css";
	import { navigating } from "$app/stores";
	import nProgress from "nprogress";
	nProgress.configure({
		minimum: 0.16,
		showSpinner: false
	});

	$: {
		if ($navigating) {
			nProgress.start();
		}
		if (!$navigating) {
			nProgress.done();
		}
	}
</script>

<slot></slot>