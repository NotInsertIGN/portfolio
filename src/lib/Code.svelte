<script>
	import { onMount } from 'svelte';
	export let language;
	export let code;
	onMount(() => {
		let script = document.createElement('script');
		script.src = "https://tutsplus.github.io/syntax-highlighter-demos/highlighters/Prism/prism.js";
		document.head.append(script);
		script.onload = () => {
			let languageJS = false;
			let languageScript;
			let languageModule;
			switch (language) {
				case "java":
					languageModule = "https://prismjs.com/components/prism-java.js";
					languageJS = true;
					break;
				case "json":
					languageModule = "https://prismjs.com/components/prism-json.js";
					languageJS = true;
					break;
				case "python":
					languageModule = "https://prismjs.com/components/prism-python.js";
					languageJS = true;
					break;
				case "rust":
					languageModule = "https://prismjs.com/components/prism-rust.js";
					languageJS = true;
					break;
			}
			if (languageJS === true) {
				languageScript = document.createElement('script');
				languageScript.src = languageModule;
				languageScript.async = true;
				document.head.append(languageScript);
				languageScript.onload = () => {
					Prism.highlightAll();
				}
			} else {
				Prism.highlightAll();
			}
		};
	});
</script>

<div class="code-container">
	<pre><code class="language-{language}">{code}</code></pre>
</div>

<svelte:head>
	<link rel="stylesheet" href='/themes/one-dark.css'>
</svelte:head>