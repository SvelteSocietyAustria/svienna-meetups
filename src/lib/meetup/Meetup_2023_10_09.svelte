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
	<p>09 / 10 / 2023</p>
	<p>Starts at 18:30</p>
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
	<p>3 Runes</p>
	<ul>
		<li>$state</li>
		<li>$derived</li>
		<li>$effect</li>
	</ul>
</Slide>

<Slide animate>
	<span class="flex" style="font-size: smaller">
		<Code id="code" lines="2|5,6,7">
			{`
			<script>
				let count = 0
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}
			</button>
		`}
		</Code>
	</span>
</Slide>

<Slide animate>
	<span class="flex" style="font-size: smaller">
		<Code id="code" lines="2-4">
			{`
			<script>
				let count = 0

				$: double = count * 2
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
	</span>
</Slide>

<Slide animate>
	<span class="flex" style="font-size: smaller">
		<Code id="code" lines="2-4">
			{`
			<script>
				let count = 0

				$: double = count * 2
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
		<Code id="code" lines="2-4">
			{`
			<script>
				let count = $state(0)

				let double = $derived(count * 2)
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
	</span>
</Slide>

<Slide animate>
	<span class="flex" style="font-size: smaller">
		<Code id="code" lines="2,8">
			{`
			<script>
				import { browser } from "$app/environment"
				
				let count = 0

				$: double = count * 2

				$: browser && console.log(double)
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
		<Code id="code" lines="3">
			{`
			<script>
				let count = $state(0)

				let double = $derived(count * 2)
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
	</span>
</Slide>

<Slide animate>
	<span class="flex" style="font-size: smaller">
		<Code id="code" lines="7">
			{`
			<script>
				import { browser } from "$app/environment"
				
				let count = 0

				$: double = count * 2

				$: browser && console.log(double)
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
		<Code id="code" lines="6-8">
			{`
			<script>
				let count = $state(0)

				let double = $derived(count * 2)

				$effect(() => {
					console.log(double);
				});
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
	</span>
</Slide>

<Slide animate>
	<span class="flex" style="font-size: smaller">
		<Code id="code" lines="7">
			{`
			<script>
				import { browser } from "$app/environment"
				
				let count = 0

				$: double = count * 2

				$: browser && console.log(double)
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
		<Code id="code" lines="6-8">
			{`
			<script>
				let count = $state(0)

				let double = $derived(count * 2)

				$effect(() => {
					console.log(double);
				});
			</script>

			<button on:click={()=>{count++}}>
				clicks: {count}, {double}
			</button>
		`}
		</Code>
	</span>
	<span class="flex">
		<p>js output: 95 lines</p>
		<p>js output: 24 lines</p>
	</span>
</Slide>

<Slide>
	<img src={Svelte5} alt="Svelte5" />
</Slide>

<Slide>
	<p>3 Runes</p>
	<ul>
		<li>✅ $state</li>
		<li>✅ $derived</li>
		<li>✅ $effect</li>
	</ul>
</Slide>

<Slide animate>
	<p>Runes</p>
	<ul>
		<li>It's early announcement</li>
		<li>They ask for feedback</li>
		<li>Things can evolves</li>
	</ul>
</Slide>

<Slide animate>
	<p>Runes</p>
	<br />
	<p>What do 🫵 think?</p>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>22 / 01 / 2024</p>
</Slide>

<style>
	.flex {
		display: flex;
		gap: 3rem;
		align-items: center;
		justify-content: center;
	}
</style>
