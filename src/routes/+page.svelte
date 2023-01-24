<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';

</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

		to<br />COVENTREE<br />Grove
	</h1>

	<h2>
		PLANNING: needs an input box with a hint that reads "lost your key? ask a member for a copy..."
	</h2>

	<h2>
		PLANNING: COVENTREE, COVEN3, C0V3NTR33, each should unlock a different experience, passed through markdown, stored in browser on request, cleared from browser on request, in this way the site can be configured differently by different users and shared with their associates and their affiliates without necessarily pushing the changes to whomever is hosting the grove (though if a particular configuration genrates enough traffic, its uuid will be on record and the grove hosts could offer to purchase or license the particular configuration)
	</h2>

	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
