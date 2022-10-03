<script>
	import Code from '../../lib/Code.svelte';
	import Giscus from '../../lib/giscus/Giscus.svelte';

	const source = `
		public class Main {
			public static void main(String[] args) {
				System.out.println("Hello, world!");
			}
		}`;
</script>

<main>
	<div class='wrapper'>
		<Code language='java' code={source}></Code>
	</div>
	<Giscus></Giscus>
</main>

<style>
    .wrapper {
        width: 50%;
    }
</style>