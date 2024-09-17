<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Code from '../deck/code.svelte'
	import Markdown from '../deck/markdown.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'
	import Ivan from '$lib/assets/IVAN.jpg'
	import Svelte5 from '$lib/assets/Svelte5.png'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>17 / 09 / 2024</p>
	<p>Starts at 18:30</p>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<br />
		<li>
			How to embrace Zod in your SvelteKit applications for schema validation and type safety by
			Sasan Jaghori
		</li>
		<li>Why the Svelte 5 API looks the way it does today by Simon Holthausen</li>
		<li>Dates - an intersection of a romantic story and Dates in JS by Domenik Reitzner</li>
		<br />
		<li>Socialize</li>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>09 / 12 / 2024</p>
	<p style="font-size: small;">https://www.meetup.com/svelte-society-austria/</p>
</Slide>

<style>
	.flex {
		display: flex;
		gap: 3rem;
		align-items: center;
		justify-content: center;
	}

	li {
		margin-bottom: 2rem;
		font-size: 2rem;
	}
</style>
