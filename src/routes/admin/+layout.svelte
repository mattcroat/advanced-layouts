<script lang="ts">
	import { Visualize } from '$lib/devtools'
</script>

<Visualize layout="admin">
	<header>
		<nav>
			<ul>
				<li>
					<a href="/">🏠️ Plume</a>
				</li>
				<li>
					<a href="/admin/analytics">📊 Analytics</a>
				</li>
				<li>
					<a href="/admin/settings">⚙️ Settings</a>
				</li>
			</ul>
		</nav>
	</header>

	<main class="space" style:--space="2rem">
		<slot />
	</main>
</Visualize>

<style>
	header {
		border-bottom: 1px solid hsl(206 29% 20%);
		padding-inline: 1rem;
	}

	main {
		padding-inline: 1rem;
	}
</style>
