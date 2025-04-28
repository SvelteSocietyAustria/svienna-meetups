<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'
	import svelte_summit_2025 from '$lib/assets/2024_12_16/svelte-summit.png'
	import svelte_summit_2025_qr from '$lib/assets/2024_12_16/Svelte_summit_Spring_2025.png'

	import advent_of_svelte_blog_qr from '$lib/assets/2024_12_16/advent_of_svelte_blog_qr.png'
	import advent_of_svelte_blog from '$lib/assets/2024_12_16/advent_of_svelte_blog.png'

	import advent_of_svelte_challange_qr from '$lib/assets/2024_12_16/advent_of_svelte_challange_qr.png'
	import advent_of_svelte_challange from '$lib/assets/2024_12_16/advent_of_svelte_challange.png'

	import logoAots from '$lib/assets/Logo-aots.svg'
	import logoLeanCoders from '$lib/assets/Logo-LeanCoders.svg'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>28 / 04 / 2025</p>
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
		<li>Intro</li>
		<span class="text-center">Svelte Summit 2025</span>
		<div class="flex justify-between gap-4 w-full">
			<img src={svelte_summit_2025} class="w-1/3" alt="svelte summit 2024" />
			<img src={svelte_summit_2025_qr} class="w-1/3" alt="svelte summit 2024 QR code" />
		</div>
	</ul>
</Slide>

<!-- <Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<span>Hosts</span>
		<div class="flex justify-between gap-4 w-full">
			<img src={logoAots} class="w-1/3" alt="aots" />
			<img src={logoLeanCoders} class="w-1/3" alt="lean coders" />
		</div>
	</ul>
</Slide> -->

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Talks</li>
		<br />
		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/30938967?v=4'}
				alt="Domenik Reitzner"
				class="avatar"
			/>
			<div class="talk-info">
				<div>Using SvelteKit and MIT appinventor to inspire young girls for tech.</div>
				<div class="speaker-name">Domenik Reitzner</div>
			</div>
		</span>

		<!-- <span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- small break --</span> -->

		<span class="speaker">
			<img src={'https://avatars.githubusercontent.com/u/5312607?v=4'} alt="JYC" class="avatar" />
			<div class="talk-info">
				<div>Lightning talk: 10 tips in 5 mins!</div>
				<div class="speaker-name">Jean-Yves Couët</div>
			</div>
		</span>

		<span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- small break --</span>

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/8420481?v=4'}
				alt="Lukas Stracke"
				class="avatar"
			/>
			<div class="talk-info">
				<div>Tracing the Slowdown: OpenTelemetry In SvelteKit Made Easy</div>
				<div class="speaker-name">Lukas Stracke</div>
			</div>
		</span>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>23 / 06 / 2025 ?</p>
	<p style="font-size: small;">https://www.meetup.com/svelte-society-austria/</p>
</Slide>

<style>
	.small-break {
		font-size: small;
		margin-top: 2rem;
		color: #666;
	}

	.flex {
		display: flex;
		gap: 3rem;
		align-items: center;
		justify-content: center;
	}

	li {
		margin-bottom: 1.5rem;
		font-size: 1.5rem;
	}

	.speaker {
		display: flex;
		align-items: center;
		gap: 0.75rem;
		font-size: 1.25rem;
		margin-bottom: 0.5rem;
	}

	.avatar {
		width: 40px;
		height: 40px;
		border-radius: 50%;
		object-fit: cover;
	}

	.talk-info {
		display: flex;
		flex-direction: column;
		gap: 0.25rem;
	}

	.speaker-name {
		font-size: 0.875rem;
		color: #666;
	}
</style>
