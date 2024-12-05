<script>
	import { GithubCorner } from '$lib';
	import Highlight from 'svelte-highlight';
	import typescript from 'svelte-highlight/languages/typescript';
	import bash from 'svelte-highlight/languages/bash';
	import github from 'svelte-highlight/styles/github-dark';

	const code = `<script>
	import { GithubCorner } from 'svelte-github-corner';
<\/script>

<GithubCorner
	href="https://github.com/flo-bit/svelte-github-corner"
	color="#fff"
	backgroundColor="#151513"
/>`;

	const installCode = `npm install svelte-github-corner`;

	const tailwindCode = `<script>
	import { GithubCorner } from 'svelte-github-corner';
<\/script>

<GithubCorner
	href="https://github.com/flo-bit/svelte-github-corner"
	class="fill-stone-900 text-stone-100 dark:fill-stone-100 dark:text-stone-900"
/>`;
</script>

<svelte:head>
	{@html github}

	<style>
		.hljs {
			background: #0c0a09 !important;
		}

		.dark .hljs {
			background: #0c0a09 !important;
		}
	</style>
</svelte:head>

<div class="relative mx-auto my-24 max-w-3xl px-4 text-stone-900 dark:text-stone-100">
	<h1 class="text-4xl font-bold">Svelte Github Corner Icon</h1>

	<div class="font-sm mt-8">
		simple little component for adding a github corner icon to your svelte projects
	</div>

	<div class="mt-6 font-bold">1. install</div>
	<div class="mt-2 overflow-hidden rounded-xl">
		<Highlight language={bash} code={installCode} />
	</div>

	<div class="mt-6 font-bold">
		2. use like this (colors are optional, will default to white on black):
	</div>
	<div class="mt-2 overflow-hidden rounded-xl">
		<Highlight language={typescript} {code} />
	</div>

	<div class="mt-6 font-bold">or use with tailwind (fill is background, text is icon):</div>
	<div class="mt-2 overflow-hidden rounded-xl">
		<Highlight language={typescript} code={tailwindCode} />
	</div>
</div>

<GithubCorner
	href="https://github.com/flo-bit/svelte-github-corner"
	class="fill-stone-900 text-stone-100 dark:fill-stone-100 dark:text-stone-900"
/>
