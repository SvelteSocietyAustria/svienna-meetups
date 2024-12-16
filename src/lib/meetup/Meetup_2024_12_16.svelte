<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'
	import svelte_summit_2025 from '$lib/assets/2024_12_16/svelte-summit.png'
	import svelte_summit_2025_qr from '$lib/assets/2024_12_16/Svelte_summit_Spring_2025.png'

	import advent_of_svelte_blog_qr from '$lib/assets/2024_12_16/advent_of_svelte_blog_qr.png'
	import advent_of_svelte_blog from '$lib/assets/2024_12_16/advent_of_svelte_blog.png'

	import advent_of_svelte_challange_qr from '$lib/assets/2024_12_16/advent_of_svelte_challange_qr.png'
	import advent_of_svelte_challange from '$lib/assets/2024_12_16/advent_of_svelte_challange.png'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>16 / 12 / 2024</p>
	<p>Starts at 18:30</p>
	<br />
	<div style="font-size: medium">🦋 @austria.sveltesociety.dev</div>
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
		<li>Intro - Svelte Summit 2025</li>
		<div style="display: flex; gap: 1rem; align-items: center;">
			<img src={svelte_summit_2025} style="width: 50%" alt="svelte summit 2024" />
			<img src={svelte_summit_2025_qr} style="width: 50%" alt="svelte summit 2024" />
		</div>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro - Advent of Svelte once a day</li>
		<div style="display: flex; gap: 1rem; align-items: center;">
			<img src={advent_of_svelte_blog} style="width: 50%" alt="svelte summit 2024" />
			<img src={advent_of_svelte_blog_qr} style="width: 50%" alt="svelte summit 2024" />
		</div>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro - Advent of Svelte challange</li>
		<div style="display: flex; gap: 1rem; align-items: center;">
			<img src={advent_of_svelte_challange} style="width: 50%" alt="svelte summit 2024" />
			<img src={advent_of_svelte_challange_qr} style="width: 50%" alt="svelte summit 2024" />
		</div>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Talks</li>
		<br />
		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/8420481?v=4'}
				alt="Lukas Stracke"
				class="avatar"
			/>
			Astro for Svelte Developers
		</span>

		<span>&nbsp;</span>
		<span style="float: right;">-- small break --</span>

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
				src={'https://avatars.githubusercontent.com/u/9527076?v=4'}
				alt="lmarti17"
				class="avatar"
			/>
			Recreating Instagram-style stories with Svelte
		</span>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>03 / 02 / 2025 ?</p>
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
