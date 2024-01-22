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
	<p>22 / 01 / 2024</p>
	<p>Starts at 18:30</p>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<br />
		<li>Using SvelteKit to build an interactive portfolio</li>
		<li>A brief history of prototyping</li>
		<li>Building an Error and Performance Monitoring SDK for SvelteKit</li>
		<li>Are you on right route?</li>
		<br />
		<li>Socialize</li>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>08 / 04 / 2024</p>
	<p style="font-size: small;">https://www.meetup.com/svelte-society-austria/</p>
</Slide>

<style>
	.flex {
		display: flex;
		gap: 3rem;
		align-items: center;
		justify-content: center;
	}
</style>
