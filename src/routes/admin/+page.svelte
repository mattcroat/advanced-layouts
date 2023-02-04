<script lang="ts">
	import { enhance } from '$app/forms'
</script>

<form method="POST" class="space" use:enhance>
	<div>
		<label for="text">
			Quote
			<textarea name="text" id="text" rows="4" required />
		</label>
	</div>

	<div>
		<label for="author">
			Author
			<input
				type="text"
				name="author"
				id="author"
				required
			/>
		</label>
	</div>

	<div>
		<label for="source">
			Source
			<input
				type="text"
				name="source"
				id="source"
				required
			/>
		</label>
	</div>

	<div>
		<label for="tags">
			Tags
			<input type="text" name="tags" id="tags" />
		</label>
	</div>

	<button type="submit">Submit Quote</button>
</form>

<style>
	form {
		max-width: 600px;
		margin-inline: auto;
	}
</style>
