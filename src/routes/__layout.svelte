<script>
	let isBurgerOpen = false;
</script>

<nav class="navbar">
	<div class="navbar-brand">
		<a class="navbar-item" href="/">
			<img src="/icon.png" alt="Caffeinated Creators" style="height: 52px; max-height: none;" />
		</a>
		<div
			class="navbar-burger"
			data-target="navbarBurger"
			on:click={() => {
				isBurgerOpen = !isBurgerOpen;
			}}
		>
			<span />
			<span />
			<span />
		</div>
	</div>

	<div
		id="navbarBurger"
		class="navbar-menu"
		class:is-active={isBurgerOpen}
		style="background-color: transparent;"
	>
		<div class="navbar-end">
			<div class="navbar-item">
				<div class="field is-grouped">
					<p class="control">
						<a class="button" href="https://twitter.com/TheCafCreators">
							<span class="icon">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="feather feather-twitter"
									><path
										d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"
									/></svg
								>
							</span>
						</a>
					</p>
					<p class="control">
						<a class="button" href="https://caf.tv/CaffeinatedCreators">
							<span class="icon">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									version="1.0"
									width="635.000000pt"
									height="635.000000pt"
									viewBox="0 0 635.000000 635.000000"
									preserveAspectRatio="xMidYMid meet"
								>
									<g
										transform="translate(0.000000,635.000000) scale(0.100000,-0.100000)"
										fill="currentColor"
										stroke="none"
									>
										<path
											d="M1594 5924 c-25 -12 -139 -202 -710 -1191 -947 -1641 -874 -1512 -874 -1553 0 -26 21 -72 78 -171 42 -74 392 -680 777 -1347 608 -1053 703 -1214 731 -1227 28 -13 216 -15 1579 -15 1363 0 1551 2 1579 15 28 13 123 174 731 1227 385 667 735 1273 778 1347 56 99 77 145 77 171 0 41 73 -88 -874 1553 -591 1023 -684 1179 -712 1192 -28 13 -216 15 -1581 15 -1359 0 -1552 -2 -1579 -16z m2610 -243 c-10 -10 -1500 -871 -1507 -871 -7 0 -757 867 -757 874 0 3 512 6 1137 6 675 0 1133 -4 1127 -9z m-2064 -620 c182 -211 330 -384 328 -386 -2 -2 -632 -364 -680 -392 -5 -2 -8 265 -8 594 0 512 2 595 14 583 8 -8 163 -188 346 -399z m1739 -407 c-253 -439 -462 -800 -464 -802 -4 -4 -1379 260 -1387 267 -4 3 514 306 1150 673 635 367 1157 666 1159 664 2 -2 -204 -363 -458 -802z m-2349 78 l0 -599 -517 -298 c-285 -164 -522 -300 -527 -303 -4 -2 -1 6 7 19 8 13 218 377 467 809 537 932 559 970 565 970 3 0 5 -269 5 -598z m3038 -1414 l-3 -671 -458 529 c-253 291 -461 534 -464 541 -3 7 204 373 459 815 l463 803 3 -673 c1 -369 1 -974 0 -1344z m838 1015 c306 -530 554 -966 552 -969 -4 -3 -1079 199 -1120 212 -17 5 -18 56 -18 882 1 764 2 875 15 858 8 -10 265 -453 571 -983z m-2692 -608 c384 -74 700 -136 701 -137 107 -119 934 -1082 931 -1085 -4 -4 -1356 253 -1392 265 -17 5 -920 1035 -948 1081 -4 6 -4 11 1 11 4 0 323 -61 707 -135z m-1184 -291 l0 -396 -22 5 c-13 3 -237 47 -498 97 -261 50 -483 94 -493 98 -13 5 111 82 485 299 277 160 509 292 516 292 9 1 12 -84 12 -395z m735 -274 c240 -278 439 -510 442 -517 4 -10 -892 -1579 -918 -1607 -5 -6 -9 573 -9 1334 l0 1345 24 -25 c13 -14 221 -252 461 -530z m3075 60 c261 -50 483 -94 493 -98 14 -5 -108 -80 -484 -297 -276 -160 -508 -291 -515 -293 -12 -3 -14 61 -14 392 l0 396 23 -5 c12 -3 236 -46 497 -95z m-4370 -330 c289 -56 533 -103 543 -106 16 -5 17 -56 17 -882 0 -549 -4 -872 -9 -866 -11 10 -1120 1930 -1129 1952 -4 11 2 13 24 8 16 -3 265 -51 554 -106z m4843 -157 c-31 -54 -263 -456 -515 -893 -253 -437 -463 -799 -469 -804 -5 -6 -9 214 -9 590 l0 601 523 301 c287 166 523 302 524 302 1 0 -23 -44 -54 -97z m-2168 -358 c369 -70 673 -131 677 -134 4 -3 -514 -306 -1150 -673 -635 -367 -1157 -666 -1159 -664 -2 2 205 364 459 805 396 685 466 802 483 798 11 -2 322 -61 690 -132z m923 -1185 l-3 -301 -343 397 c-274 317 -341 399 -328 406 8 5 163 94 343 198 l328 189 3 -294 c1 -161 1 -429 0 -595z m-534 -74 c207 -239 376 -437 376 -440 0 -3 -512 -6 -1137 -6 -625 0 -1133 3 -1129 8 10 9 1499 871 1507 872 4 0 176 -195 383 -434z"
										/>
									</g>
								</svg>
							</span>
						</a>
					</p>
					<p class="control">
						<a class="button" href="/discord">
							<span class="icon">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									fill-rule="evenodd"
									clip-rule="evenodd"
									viewBox="0 0 24 24"
									fill="currentColor"
								>
									<path
										d="M19.54 0c1.356 0 2.46 1.104 2.46 2.472v21.528l-2.58-2.28-1.452-1.344-1.536-1.428.636 2.22h-13.608c-1.356 0-2.46-1.104-2.46-2.472v-16.224c0-1.368 1.104-2.472 2.46-2.472h16.08zm-4.632 15.672c2.652-.084 3.672-1.824 3.672-1.824 0-3.864-1.728-6.996-1.728-6.996-1.728-1.296-3.372-1.26-3.372-1.26l-.168.192c2.04.624 2.988 1.524 2.988 1.524-1.248-.684-2.472-1.02-3.612-1.152-.864-.096-1.692-.072-2.424.024l-.204.024c-.42.036-1.44.192-2.724.756-.444.204-.708.348-.708.348s.996-.948 3.156-1.572l-.12-.144s-1.644-.036-3.372 1.26c0 0-1.728 3.132-1.728 6.996 0 0 1.008 1.74 3.66 1.824 0 0 .444-.54.804-.996-1.524-.456-2.1-1.416-2.1-1.416l.336.204.048.036.047.027.014.006.047.027c.3.168.6.3.876.408.492.192 1.08.384 1.764.516.9.168 1.956.228 3.108.012.564-.096 1.14-.264 1.74-.516.42-.156.888-.384 1.38-.708 0 0-.6.984-2.172 1.428.36.456.792.972.792.972zm-5.58-5.604c-.684 0-1.224.6-1.224 1.332 0 .732.552 1.332 1.224 1.332.684 0 1.224-.6 1.224-1.332.012-.732-.54-1.332-1.224-1.332zm4.38 0c-.684 0-1.224.6-1.224 1.332 0 .732.552 1.332 1.224 1.332.684 0 1.224-.6 1.224-1.332 0-.732-.54-1.332-1.224-1.332z"
									/>
								</svg>
							</span>
						</a>
					</p>
				</div>
			</div>
		</div>
	</div>
</nav>

<div id="page-content">
	<slot />
</div>

<footer class="footer">
	<div class="content has-text-centered">
		<p>Brought to you with ♥ by all of us at the Caffeinated Creators.</p>
	</div>

	<div class="tabs is-centered">
		<ul>
			<li>
				<a href="/discord">Discord</a>
			</li>
			<li>
				<a href="https://caffeine.tv/CaffeinatedCreators">Stream</a>
			</li>
			<li>
				<a href="https://twitter.com/TheCafCreators">Twitter</a>
			</li>
		</ul>
	</div>

	<!-- Plausible -->
	<script
		defer
		data-domain="caffeinatedcreators.cc"
		src="https://plausible.io/js/plausible.js"></script>
</footer>

<style>
	#page-content {
		min-height: 100vh;
	}

	nav {
		position: fixed;
		top: 0;
		left: 0;
		right: 0;
		background-color: transparent;
	}
</style>
