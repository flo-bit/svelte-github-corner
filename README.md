# svelte-github-corner

simple little component for adding a github corner icon to your svelte projects

[see it in action](https://flo-bit.dev/svelte-github-corner/)

## install

```bash
npm install svelte-github-corner
```

## use

- the colors are optional, will default to black on white

```svelte
<script>
	import { GithubCorner } from 'svelte-github-corner';
<\/script>

<GithubCorner
	href="https://github.com/flo-bit/svelte-github-corner"
	color="#fff"
	backgroundColor="#151513"
/>
```

### using with tailwind

- fill is background, text is icon

```svelte
<script>
	import { GithubCorner } from 'svelte-github-corner';
<\/script>

<GithubCorner
	href="https://github.com/flo-bit/svelte-github-corner"
	class="fill-stone-900 text-stone-100 dark:fill-stone-100 dark:text-stone-900"
/>
```

## license

MIT

## credits

based on [github corners](https://github.com/tholman/github-corners) by Tim Holman