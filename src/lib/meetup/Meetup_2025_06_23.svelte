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
	<p>23 / 06 / 2025</p>
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
		<div class="w-full p-4">
			<a class="link" href="https://www.svelte.at/">svelte.at</a>
		</div>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<span>Hosts</span>
		<div class="flex justify-between gap-4 w-full">
			<img src={logoAots} class="w-1/3" alt="aots" />
			<img src={logoLeanCoders} class="w-1/3" alt="lean coders" />
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
				src={'https://avatars.githubusercontent.com/u/465547?v=4'}
				alt="Martin Grubinger"
				class="avatar"
			/>
			<div class="talk-info">
				<div>Svelte at Geizhals</div>
				<div class="speaker-name">Martin Grubinger</div>
			</div>
		</span>

		<!-- <span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- small break --</span> -->

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/10669513?v=4'}
				alt="derharry"
				class="avatar"
			/>
			<div class="talk-info">
				<div>ZeeltePHP (Svelte + PHP)</div>
				<div class="speaker-name">derharry</div>
			</div>
		</span>

		<span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- Pizza Break --</span>

		<span class="speaker">
			<img src={'https://avatars.githubusercontent.com/u/5312607?v=4'} alt="JYC" class="avatar" />
			<div class="talk-info">
				<div>Adding full to your full-stack SvelteKit app</div>
				<div class="speaker-name">Jean-Yves Couët</div>
			</div>
		</span>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>16 / 09 / 2025 ?</p>
	<p style="font-size: small;">https://svelte.at</p>
	<p style="font-size: small;">https://www.meetup.com/svelte-society-austria</p>
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
