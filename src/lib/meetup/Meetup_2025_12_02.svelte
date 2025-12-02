<script lang="ts">
	import Slide from '../deck/slide.svelte'
	import Logo from '$lib/assets/Logo-Dark-Tagline.svg'
	import logoSentry from '$lib/assets/Logo-sentry.svg'
</script>

<Slide>
	<span class="flex">
		<p>👋 Welcome to</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>02 / 12 / 2025</p>
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
		<span>Hosts</span>
		<div class="flex justify-between gap-4 w-full">
			<img src={logoSentry} class="w-1/3" alt="sentry" />
		</div>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Intro</li>
		<ul>
			<li>Code of Conduct</li>
			<ul>
				<li>Be nice to each other!</li>
				<li>Reach out to us if needed</li>
				<li>
					<a class="link" href="https://www.svelte.at/code-of-conduct">svelte.at/code-of-conduct</a>
				</li>
			</ul>
		</ul>
	</ul>
</Slide>

<Slide id="list" animate>
	<p>What's up today?</p>
	<ul>
		<li>Talks</li>
		<br />

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/76689341?v=4'}
				alt="Housein Abo Shaar"
				class="avatar"
			/>
			<div class="talk-info">
				<div>Svelte Under the Hood</div>
				<div class="speaker-name">Housein Abo Shaar</div>
			</div>
		</span>

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/5202322?v=4'}
				alt="danirukun"
				class="avatar"
			/>
			<div class="talk-info">
				<div>How Svelte took over Apple - lessons from the App Store</div>
				<div class="speaker-name">danirukun</div>
			</div>
		</span>

		<span>&nbsp;</span>
		<span style="float: right;" class="small-break">-- 20 min Break --</span>

		<span class="speaker">
			<img
				src={'https://avatars.githubusercontent.com/u/2931?v=4'}
				alt="Michael Aufreiter"
				class="avatar"
			/>
			<div class="talk-info">
				<div>CMS-Free, Editable Websites with Svelte and Svedit</div>
				<div class="speaker-name">Michael Aufreiter</div>
			</div>
		</span>
	</ul>
</Slide>

<Slide>
	<span class="flex">
		<p>👋 See you next time</p>
		<img width="200" alt="logo" src={Logo} />
	</span>
	<p>24 / 02 / 2026 ?</p>
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
