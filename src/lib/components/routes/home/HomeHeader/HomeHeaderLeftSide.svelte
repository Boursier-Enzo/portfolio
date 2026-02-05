<div class="left-side">
	<h1 class="left-side__main-title">FULL STACK DEVELOPER</h1>
	<h2 class="left-side__second-title">Hello, World. I am Enzo.</h2>
	<div class="left-side__paragraph">
		<div class="left-side__paragraph__line"></div>
		<p class="left-side__paragraph__text">
			Passionate about turning complex challenges into simple, elegant solutions. I create digital
			products that combine robust technology with seamless user experiences.
		</p>
	</div>
	<div class="left-side__button">
		<a class="left-side__button__project" href="#project"
			><span class="left-side__button__project__text">VIEW PROJECT</span>
			<svg
				class="left-side__button__project__icon"
				xmlns="http://www.w3.org/2000/svg"
				id="Filled"
				viewBox="0 0 24 24"
				fill="#1a2035"
			>
				<path
					d="M19,4H17.9A5.009,5.009,0,0,0,13,0H11A5.009,5.009,0,0,0,6.1,4H5A5.006,5.006,0,0,0,0,9v3H24V9A5.006,5.006,0,0,0,19,4ZM8.184,4A3,3,0,0,1,11,2h2a3,3,0,0,1,2.816,2Z"
				/>
				<path
					d="M13,15a1,1,0,0,1-2,0V14H0v5a5.006,5.006,0,0,0,5,5H19a5.006,5.006,0,0,0,5-5V14H13Z"
				/>
			</svg>
		</a><a class="left-side__button__contact" href="#contact"
			><span class="left-side__button__contact__text">CONTACT ME</span>
			<svg
				class="left-side__button__contact__icon"
				xmlns="http://www.w3.org/2000/svg"
				id="Layer__1"
				data-name="Layer 1"
				viewBox="0 0 24 24"
				fill="#00f5ff"
			>
				<path
					d="M24,23c0,.55-.45,1-1,1-1.54,0-2.29-1.12-2.83-1.95-.5-.75-.75-1.05-1.17-1.05-.51,0-.9,.44-1.51,1.15-.7,.83-1.57,1.85-3.03,1.85s-2.32-1.03-3-1.87c-.58-.7-.96-1.13-1.46-1.13-.39,0-.63,.25-1.16,.91-.72,.88-1.71,2.09-3.84,2.09-2.76,0-5-2.24-5-5s2.24-5,5-5c.55,0,1,.45,1,1s-.45,1-1,1c-1.65,0-3,1.35-3,3s1.35,3,3,3c1.18,0,1.67-.6,2.29-1.36,.6-.73,1.34-1.64,2.71-1.64,1.47,0,2.32,1.03,3,1.87,.58,.7,.96,1.13,1.46,1.13s.9-.44,1.51-1.15c.7-.83,1.57-1.85,3.03-1.85s2.29,1.12,2.83,1.95c.5,.75,.75,1.05,1.17,1.05,.55,0,1,.45,1,1Zm-15.01-7h.94c1.06,0,2.08-.42,2.83-1.17l7.72-7.72-3.59-3.59-7.72,7.72c-.75,.75-1.17,1.77-1.17,2.83v.94c0,.55,.44,.99,.99,.99ZM23.26,4.33c.48-.48,.74-1.12,.74-1.8s-.26-1.32-.74-1.79c-.99-.99-2.6-.99-3.59,0l-1.36,1.36,3.59,3.59,1.36-1.36Z"
				/>
			</svg>
		</a>
	</div>

	<div class="left-side__work-status">
		<div class="left-side__work-status__dot"></div>
		<span class="left-side__work-status__text">AVAILABLE FOR WORK</span>
	</div>
</div>

<style lang="scss">
	.left-side {
		width: 50%;
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: start;
		justify-content: center;

		@include md {
			margin-top: 10rem;
			width: 80%;
			height: auto;
			align-items: center;
		}

		& > * {
			margin-left: 3rem;

			@include md {
				margin-left: 0;
			}
		}

		&__main-title {
			width: 50%;
			max-width: 100%;
			font-size: $font-size-5xl;
			font-weight: $font-weight-bold;
			color: $text-title;
			order: 2;
			margin-top: 0.5rem;

			@include md {
				width: 100%;
				text-align: center;
			}

			@media screen and (max-width: (525px)) {
				font-size: $font-size-2xl;
				width: 23rem;
			}
		}

		&__second-title {
			font-size: $font-size-2xl;
			font-weight: $font-weight-medium;
			color: $text-code;
			order: 1;
			margin-top: 2rem;

			@media screen and (max-width: (525px)) {
				font-size: $font-size-xl;
			}
		}

		&__paragraph {
			order: 3;
			display: flex;
			align-items: center;
			margin-top: 2rem;

			@include md {
				flex-direction: column;
			}
			&__line {
				width: 0.2rem;
				height: 4rem;
				border-radius: 1rem;
				background-color: $accent-cyan;

				@include lg {
					height: 6rem;
				}

				@include md {
					width: 30rem;
					height: 0.2rem;
				}

				@media screen and (max-width: (525px)) {
					width: 20rem;
				}
			}

			&__text {
				width: 35rem;
				font-size: $font-size-lg;
				font-weight: $font-weight-regular;
				color: $text-body;
				margin-left: 1rem;
				@include lg {
					width: 25rem;
				}

				@include md {
					margin-left: 0;
					margin-top: 1rem;
				}

				@media screen and (max-width: (525px)) {
					font-size: $font-size-md;
					width: 18rem;
				}
			}
		}

		&__button {
			display: flex;
			order: 4;
			margin-top: 4rem;
			gap: 1rem;

			@media screen and (max-width: (525px)) {
				flex-direction: column;
				margin-top: 2rem;
			}
			&__project {
				display: flex;
				align-items: center;
				padding: 0.8rem 1.5rem 0.8rem 1.5rem;
				background-color: $accent-cyan;
				border: solid $text-code 0.1rem;
				border-radius: 0.3rem;
				text-decoration: none;
				color: $bg-secondary;
				box-shadow: 0 0 0.5rem $accent-cyan;
				transition: box-shadow 0.5s ease-in-out;
				gap: 0.5rem;

				&__icon {
					width: 1rem;
					height: 1rem;
				}

				@media (hover: hover) {
					&:hover {
						box-shadow: 0 0 1rem $accent-cyan;
					}
				}
			}
			&__contact {
				display: flex;
				align-items: center;
				padding: 0.8rem 1.5rem 0.8rem 1.5rem;
				border: solid $text-code 0.1rem;
				border-radius: 0.3rem;
				text-decoration: none;
				color: $text-code;
				box-shadow: 0 0 0.5rem $accent-cyan;
				transition: box-shadow 0.5s ease-in-out;
				gap: 0.5rem;

				&__icon {
					width: 1rem;
					height: 1rem;
				}

				@media (hover: hover) {
					&:hover {
						box-shadow: 0 0 1rem $accent-cyan;
					}
				}
			}
		}

		&__work-status {
			display: flex;
			align-items: center;
			background-color: #141a28;
			padding: 0.6rem 1.2rem 0.6rem 1.2rem;
			border-radius: 1rem;
			border: solid 0.01rem $accent-cyan;
			order: 0;

			&__dot {
				width: 1rem;
				height: 1rem;
				background-color: $accent-cyan;
				border-radius: 1rem;
				@media screen and (max-width: (525px)) {
					width: 0.8rem;
					height: 0.8rem;
				}
			}

			&__text {
				margin-left: 1rem;
				color: $text-code;

				@media screen and (max-width: (525px)) {
					font-size: $font-size-xs;
				}
			}
		}
	}
</style>
