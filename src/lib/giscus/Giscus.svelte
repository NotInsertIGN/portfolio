<script lang="ts">
	import { onMount } from 'svelte';
	import type {
		AvailableLanguage,
		BooleanString,
		InputPosition,
		Loading,
		Mapping,
		Theme,
	} from '..';

	export let id: string = undefined;
	export let host = 'https://giscus.app';
	export let repo: `${string}/${string}` = "neopixeldev/hypixel-api-java";
	export let repoId: string = "R_kgDOHn_PPg";
	export let category: string = "Announcements";
	export let categoryId: string = "DIC_kwDOHn_PPs4CQJYu";
	export let mapping: Mapping = 'specific';
	export let term: string = "Welcome to @giscus/svelte component!";
	export let strict: BooleanString = "1";
	export let reactionsEnabled: BooleanString = '1';
	export let emitMetadata: BooleanString = '0';
	export let inputPosition: InputPosition = 'top';
	export let theme: Theme = 'dark';
	export let lang: AvailableLanguage = 'en';
	export let loading: Loading = 'eager';

	let mounted = false;

	onMount(() => {
		mounted = true;
		import('giscus');
	});
</script>

{#if mounted}
	<giscus-widget
		{id}
		{host}
		{repo}
		repoid={repoId}
		{category}
		categoryid={categoryId}
		{mapping}
		{term}
		{strict}
		reactionsenabled={reactionsEnabled}
		emitmetadata={emitMetadata}
		inputposition={inputPosition}
		{theme}
		{lang}
		{loading}>
	</giscus-widget>
{/if}