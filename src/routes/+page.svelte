<div class="hero space">
	<div class="title">
		<h1 class="serif capitalize">
			Find and share memorable quotes that inspire you
		</h1>
	</div>

	<div class="quote">
		<article>
			<p class="serif">“What, You Egg!” — Shakespeare</p>

			<div class="tags">
				<a href="/quotes/tags/drama">#drama</a>
			</div>

			<footer>
				<a href="/quotes/id/1234">Share →</a>
			</footer>
		</article>
	</div>
</div>

<style>
	.hero {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		grid-template-rows: repeat(4, 140px);
	}

	.hero::after {
		content: '';
		grid-row: 1 / -1;
		grid-column: 3 / -1;
		background-image: url('cover.jpg');
		background-size: cover;
		border-radius: 1rem;
		z-index: -10;
	}

	.title {
		height: 100%;
		grid-column: 1 / 4;
		grid-row: 1 / 3;
		display: grid;
		place-content: center;
	}

	.quote {
		grid-column: 1 / 4;
		grid-row: 3;
	}

	article {
		margin: 0;
	}
</style>
