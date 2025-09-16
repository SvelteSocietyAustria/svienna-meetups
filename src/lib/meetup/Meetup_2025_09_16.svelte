<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'

	import vite_conf_2025 from '$lib/assets/2025_09_16/vite-conf.png'

	import logoAots from '$lib/assets/Logo-aots.svg'
	import logoLeanCoders from '$lib/assets/Logo-LeanCoders.svg'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>16 / 09 / 2025</p>
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
		<img src={vite_conf_2025} alt="Vite Conf 2025" />
		<center> Raffle </center>
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
				src={'https://avatars.githubusercontent.com/u/9217404?v=4'}
				alt="Jacob Palecek"
				class="avatar"
			/>
			<div class="talk-info">
				<div>Svelte and LLMs - A Token Effort</div>
				<div class="speaker-name">Jacob Palecek</div>
			</div>
		</span>

		<!-- <span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- small break --</span> -->

		<span class="speaker">
			<img src={'https://avatars.githubusercontent.com/u/5312607?v=4'} alt="JYC" class="avatar" />
			<div class="talk-info">
				<div>💡 Lightning talk: do you know "sv"?</div>
				<div class="speaker-name">Jean-Yves Couët</div>
			</div>
		</span>

		<span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- Break --</span>

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/30938967?v=4'}
				alt="Domenik Reitzner"
				class="avatar"
			/>
			<div class="talk-info">
				<div>Async ⏳ Svelte</div>
				<div class="speaker-name">Domenik Reitzner</div>
			</div>
		</span>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>dd / MM / 2025 ?</p>
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
