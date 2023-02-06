<script lang="ts">
	import Visualize from '$lib/components/visualize.svelte'
</script>

<h2 class="serif space">Dashboard</h2>

<Visualize layout="admin">
	<slot />
</Visualize>
