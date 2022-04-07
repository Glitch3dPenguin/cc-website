<script>
	const LEFT_SIDE = [
		{
			handle: 'FallenWolf',
			name: 'Justin',
			avatar: '/people/FallenWolf/avatar.png',
			role: 'Founder & Streamer',
			link: 'https://caf.tv/FallenWolf'
		},
		{
			handle: 'Glitch3dPenguin',
			name: 'Max',
			avatar: '/people/Glitch3dPenguin/avatar.png',
			role: 'Founder & Streamer',
			link: 'https://caf.tv/Glitch3dPenguin'
		},
		{
			handle: 'SilverZambie',
			name: 'Mike',
			avatar: '/people/SilverZambie/avatar.png',
			role: 'Founder & Streamer',
			link: 'https://caf.tv/SilverZambie'
		}
	];

	const RIGHT_SIDE = [
		{
			handle: 'PigStand',
			name: 'Nick',
			avatar: '/people/PigStand/avatar.png',
			role: 'Streamer',
			link: 'https://caf.tv/PigStand'
		},
		{
			handle: 'AuzzieTheAussie',
			name: 'Auzzie',
			avatar: '/people/AuzzieTheAussie/avatar.png',
			role: 'Streamer',
			link: 'https://caf.tv/AuzzieTheAussie'
		},
		{
			handle: 'mcmantgp',
			name: 'Dusty',
			avatar: '/people/mcmantgp/avatar.png',
			role: 'Streamer',
			link: 'https://caf.tv/mcmantgp'
		},
		{
			handle: 'JamminJoey',
			name: 'Joey',
			avatar: '/people/JamminJoey/avatar.png',
			role: 'Streamer',
			link: 'https://caf.tv/JamminJoey'
		}
	];
</script>

<section id="welcome-wagon">
	<video src="/video/CC-PromoCut.mp4" autoplay muted loop />
</section>

<section id="name-band" class="has-text-centered">
	<div style="height: 100%; display: flex; justify-content: center; align-items: center;">
		<h1 class="title is-size-1">The Caffeinated Creators</h1>
	</div>
</section>

<section>
	<div class="card" style="border-radius: 0; box-shadow: none; width: 100%">
		<div class="columns" style="width: 80%; margin: auto;">
			<div class="column is-narrow">
				{#each LEFT_SIDE as member}
					<div class="card" style="border-radius: 0; box-shadow: none;">
						<div class="card-content">
							<div class="media">
								<div class="media-left">
									<figure class="image is-48x48">
										<img class="is-rounded" src={member.avatar} alt={member.name} />
									</figure>
								</div>
								<div class="media-content">
									<p class="title is-4">{member.name}</p>
									<p class="subtitle is-6">
										<a
											href={member.link}
											target="_blank"
											style="color: inherit; text-decoration: underline;"
										>
											@{member.handle}
										</a>
									</p>
								</div>
							</div>
						</div>
					</div>
				{/each}
			</div>
			<div class="column has-text-centered">
				<br />
				<br />
				<br />
				<h1 class="title is-size-3">
					Quite possibly the most energetic group livestreaming has ever seen. ☕
				</h1>
				<br />
			</div>
			<div class="column is-narrow">
				{#each RIGHT_SIDE as member}
					<div class="card" style="border-radius: 0; box-shadow: none;">
						<div class="card-content">
							<div class="media">
								<div class="media-content has-text-right">
									<p class="title is-4">{member.name}</p>
									<p class="subtitle is-6">
										<a
											href={member.link}
											target="_blank"
											style="color: inherit; text-decoration: underline;"
										>
											@{member.handle}
										</a>
									</p>
								</div>
								<div class="media-right">
									<figure class="image is-48x48">
										<img class="is-rounded" src={member.avatar} alt={member.name} />
									</figure>
								</div>
							</div>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>

<style>
	#welcome-wagon {
		background: black;
	}

	#welcome-wagon video {
		width: 100%;
		height: 100%;
		max-width: 100vw;
		max-height: calc(100vh - 14em);
	}

	@media (prefers-color-scheme: light) {
		.card {
			background-color: #eaeaea;
		}
	}

	#name-band {
		height: 14em;
	}

	@media (prefers-color-scheme: dark) {
		#name-band {
			color: #fafafa;
			background-color: #060606;
		}
	}
</style>
