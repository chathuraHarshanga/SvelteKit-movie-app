<script context="module">
	export async function load({ fetch, params }) {
		const res = await fetch(
			`https://api.themoviedb.org/3/movie/${params.id}?api_key=8c5b5e30e504139fd6699ba73c13557e&language=en-US`
		);
		const movieDetail = await res.json();
		if (res.ok) {
			return {
				props: { movieDetail }
			};
		}
	}
</script>

<script>
	export let movieDetail;
</script>

<div class="movie-details">
	<div class="img-container">
		<img src={'https://image.tmdb.org/t/p/original' + movieDetail.backdrop_path} alt="" srcset="" />
	</div>
	<div class="txt-container">
		<p class="overview">{movieDetail.overview}</p>
		<p>
			<span>Release date</span>
			{movieDetail.release_date} <br />
		</p>
	</div>
</div>

<style>
	p {
		padding: 1rem 0rem;
	}
	.img-container {
		width: 100%;
	}
	img {
		width: 100%;
		border-radius: 1rem;
		margin-top: 8rem;
	}
	.movie-details {
		margin: 0rem 20%;
	}
	span {
		font-weight: bold;
	}
</style>
