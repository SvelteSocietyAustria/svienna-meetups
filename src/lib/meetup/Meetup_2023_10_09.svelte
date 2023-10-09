<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Code from '../deck/code.svelte'
	import Markdown from '../deck/markdown.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'
	import Ivan from '$lib/assets/IVAN.jpg'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>09 / 10 / 2023</p>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<li>1 minute of silence</li>
		<li>Sentry presentation</li>
		<li>
			SvelteKit: From landing page to offline PWAs by Daniils Petrovs <i>(TwiX: @DaniruKun)</i>
		</li>
		<li>Panel: Svelte 5 runes the web faster by Svienna</li>
		<li>Outro</li>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<img
			width="200"
			style="border-radius: 100%;"
			alt="Ivan"
			src="https://avatars.githubusercontent.com/u/21335119?v=4"
		/>
		<img style="border-radius: 10%;" width="150" alt="Ivan" src={Ivan} />
	</span>
	<p>Ivan Hofer</p>
	<p>† 26 / 08 / 2023</p>
</Slide>

<Slide>
	<p>Sentry presentation</p>
</Slide>

<Slide>
	<p>SvelteKit: From landing page to offline PWAs by Daniils Petrovs <i>(TwiX: @DaniruKun)</i></p>
</Slide>

<Slide>
	<p>Panel: Svelte 5 runes the web faster by Svienna</p>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>dd / MM / 202y</p>
</Slide>

<style>
	.flex {
		display: flex;
		gap: 3rem;
		align-items: center;
		justify-content: center;
	}
</style>
