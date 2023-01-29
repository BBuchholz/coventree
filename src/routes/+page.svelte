<script>
	import Counter from './Counter.svelte';
	// import welcome from '$lib/images/svelte-welcome.webp';
	// import welcome_fallback from '$lib/images/svelte-welcome.png';
	import cg_logo from '$lib/images/Coventree_Grove-logos_black.png';


</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>


	<span class="welcome">
		<picture>
			<!-- <source srcset={welcome} type="image/webp" />
			<img src={welcome_fallback} alt="Welcome" /> -->
			
			<img src={cg_logo} alt="Welcome" />
		</picture>
	</span>


	<p>
		PLANNING: Create Word Art To Replace The Default WELCOME Image (should read COVENTREE [line break] Grove)
	</p>

	<p>PLANNING: this is the default layout and template of the skeleton starter app, add Bootstrap and pick a theme that feels appropriate, projeckt planning uuid (9da4313f-a9cd-498a-9972-5d4a61418060)</p>


	<p>PLANNING: "WHAT WE'RE BUILDING" - All Projeckts should have a page here, coventree is core tree, and will only be shown to those who we want to share the entire vision with, all other groves will be subsets that only directly link to coventree if apropos, projeckt planning uuid (9da4313f-a9cd-498a-9972-5d4a61418060) </p> 

	<p>
		PLANNING: add projeckt notes for Myriad Planning, which will become its own grove and be everything about the library tools, projeckt planning uuid (57fe5c68-dc12-41b9-b564-8fa8295dfc74)
	</p>

	<p>
		PLANNING: projeckt notes for MyriaD MarkDown Matrix, to become a <a href="https://tauri.app/" target="_blank" rel="noreferrer">Tauri App</a> using <a href="https://tauri.app/v1/guides/getting-started/setup/sveltekit/" target="_blank" rel="noreferrer">SvelteKit</a> as a frontend, to become our desktop component in the Sylvan Circle ecosystem, projeckt planning uuid (d7c371d8-d658-44c9-b5ed-809a2191d552)
	</p>


	<p>
		PLANNING: needs an input box with a hint that reads "lost your key? ask a member for a copy..." (not yet added to a planning doc)
	</p>

	<p>
		PLANNING: COVENTREE, COVEN3, C0V3NTR33, each should unlock a different experience, passed through markdown, stored in browser on request, cleared from browser on request, in this way the site can be configured differently by different users and shared with their associates and their affiliates without necessarily pushing the changes to whomever is hosting the grove (though if a particular configuration genrates enough traffic, its uuid will be on record and the grove hosts could offer to purchase or license the particular configuration) (not yet added to a planning doc)
	</p>

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
		width: 100%;
		height: auto;
		/* top: 0;
		display: block; */
		object-fit: cover;
		object-position: center;
	}
</style>
