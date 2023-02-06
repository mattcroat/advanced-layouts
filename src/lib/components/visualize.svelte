<script lang="ts">
	import devTools from '$lib/stores/devtools'

	export let layout: string
</script>

{#if $devTools.layout}
	<div data-layout={layout}>
		<slot />
	</div>
{:else}
	<slot />
{/if}

<style>
	[data-layout] {
		border: 8px solid aqua;
	}

	[data-layout]::before {
		content: attr(data-layout) ' layout';
		margin-left: 0.2rem;
		font-weight: bold;
		text-transform: uppercase;
		color: aqua;
	}
</style>
