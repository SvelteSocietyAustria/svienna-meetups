<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'
	import svelte_summit_2024 from '$lib/assets/2024_12_16/svelte-summit.png'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>16 / 12 / 2024</p>
	<p>Starts at 18:30</p>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<li>Talks</li>
		<li>Socialize</li>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<img src={svelte_summit_2024} alt="svelte summit 2024" />
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Talks</li>
		<br />
		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/9527076?v=4'}
				alt="lmarti17"
				class="avatar"
			/>
			Recreating Instagram-style stories with Svelte
		</span>

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/30973909?v=4'}
				alt="Sasan Jaghori"
				class="avatar"
			/>
			Deploying SvelteKit on AWS Lambda
		</span>

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/8420481?v=4'}
				alt="Lukas Stracke"
				class="avatar"
			/>
			Astro for Svelte Developers
		</span>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>10 / 02 / 2025</p>
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

	.speaker {
		display: flex;
		align-items: center;
		gap: 1rem;
	}

	.avatar {
		width: 50px;
		height: 50px;
		border-radius: 50%;
		object-fit: cover;
	}
</style>
