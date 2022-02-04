<script>
	let inputValue = '';

	import { goto } from '$app/navigation';
	function submitSearch() {
		goto('/search/' + inputValue);
	}
</script>

<form on:submit|preventDefault={submitSearch} class="search">
	<label for="search_movie">Search movies</label>
	<input bind:value={inputValue} type="text" name="search_movie" />
	<button>Search</button>
</form>

<style>
	.search {
		padding-top: 7rem;
	}
</style>
