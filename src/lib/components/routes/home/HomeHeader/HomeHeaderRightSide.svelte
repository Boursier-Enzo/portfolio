<div class="right-side">
	<div class="right-side__code-window">
		<div class="right-side__code-window__nav">
			<svg
				class="right-side__code-window__nav__icons"
				viewBox="0 0 81 21"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<g clip-path="url(#clip0__25__8)">
					<circle cx="10.5" cy="10.5" r="10.5" fill="#C53E44" />
					<circle cx="40.5" cy="10.5" r="10.5" fill="#C19714" />
					<circle cx="70.5" cy="10.5" r="10.5" fill="#21A659" />
				</g>
				<defs>
					<clipPath id="clip0__25__8">
						<rect width="81" height="21" fill="white" />
					</clipPath>
				</defs>
			</svg>
			<div class="right-side__code-window__nav__text">&lt; &gt; developer.config.ts</div>
		</div>
		<div class="right-side__code-window__main">
			<div class="code">
				<ul class="code__tab code__tab--noline">
					<li class="code__tab__line">
						<span class="code__purple">const</span>
						<span class="code__cyan">developer</span> = {'{'}
					</li>
					<ul class="code__tab">
						<li class="code__tab__line">
							<span>name:</span>
							<span class="code__green mr-0">'Enzo'</span>,
						</li>
					</ul>
					<ul class="code__tab">
						<li class="code__tab__line">
							<span>role:</span>
							<span class="code__green mr-0">'Full Stack Developer'</span>,
						</li>
					</ul>
					<ul class="code__tab">
						<li class="code__tab__line"><span>skills:</span>[</li>
						<ul class="code__tab">
							<li class="code__tab__line">
								<span class="code__green mr-0">'React'</span>,
							</li>
						</ul>

						<ul class="code__tab">
							<li class="code__tab__line">
								<span class="code__green mr-0">'Symfony'</span>,
							</li>
						</ul>
						<ul class="code__tab">
							<li class="code__tab__line">
								<span class="code__green mr-0">'Python'</span>,
							</li>
						</ul>
						<ul class="code__tab">
							<li class="code__tab__line">
								<span class="code__green mr-0">'Java'</span>,
							</li>
						</ul>
						<ul class="code__tab">
							<li class="code__tab__line">
								<span class="code__green mr-0">'SQL'</span>,
							</li>
						</ul>
					</ul>
					<ul class="code__tab">
						<li class="code__tab__line">
							<span>passionate:</span>
							<span class="code__purple mr-0">'true'</span>,
						</li>
					</ul>
					<ul class="code__tab">
						<li class="code__tab__line">
							<span>hardWorker:</span>
							<span class="code__purple mr-0">'true'</span>,
						</li>
					</ul>
					<ul class="code__tab">
						<li class="code__tab__line">
							<span>hireable:</span>
							<span class="code__purple">function</span>() {'{'}
						</li>
						<ul class="code__tab">
							<li class="code__tab__line">
								<span class="code__purple">return</span><span>
									<span class="code__cyan mr-0">this</span>.passionate &&
									<span class="code__cyan mr-0">this</span>.hardWorker;</span
								>
							</li>
						</ul>
					</ul>
					<ul class="code__tab">
						<li class="code__tab__line">
							<span>}</span>
						</li>
					</ul>
					<li class="code__tab__line">};</li>
				</ul>
			</div>
			<div class="right-side__code-window__main__terminal">
				<div class="right-side__code-window__main__terminal__path">~/dev/portfolio</div>
				<div class="right-side__code-window__main__terminal__output"></div>
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	.right-side {
		width: 50%;
		height: 100%;
		display: flex;
		align-items: center;
		justify-content: end;

		@include md {
			width: 80%;
			height: auto;
			margin-top: 5rem;
			justify-content: center;
		}
		&__code-window {
			width: 28rem;
			padding-bottom: 1rem;
			margin-right: 3rem;
			position: relative;
			border-radius: 1rem;
			background-color: $bg-secondary;

			@include md {
				margin-right: 0;
			}

			&::before {
				content: '';
				width: 100%;
				height: 100%;
				position: absolute;
				z-index: -1;
				transform: rotate(4deg) scale(0.99);
				filter: blur(0.3rem);
				opacity: 0.2;
				background: $accent-cyan;
			}

			&__nav {
				width: 100%;
				height: 3rem;
				background-color: #1e2b45;
				border-radius: 1rem 1rem 0rem 0rem;
				display: flex;
				justify-content: space-between;
				align-items: center;

				&__icons {
					width: 10%;
					margin-left: 1rem;
				}
				&__text {
					margin-right: 1rem;
					color: $text-body;

					@media screen and (max-width: (525px)) {
						font-size: $font-size-xs;
					}
				}
			}

			&__main {
				display: flex;
				flex-direction: column;

				.code {
					margin-top: 1rem;
					margin-bottom: 1rem;
					color: $text-body;
					font-size: $font-size-sm;
					font-family:
						ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono',
						monospace;

					&__purple {
						color: #c285fe;
					}

					&__cyan {
						color: #00ddff;
					}

					&__green {
						color: #4de784;
					}

					&__tab {
						border-left: 1px solid rgba(150, 150, 150, 0.3);
						padding-left: 1rem;
						list-style: none;

						&--noline {
							border-left: none;
						}

						&__line {
							height: 1.3rem;
							display: flex;
							align-items: center;

							@media screen and (max-width: (525px)) {
								height: 1rem;
							}
							span {
								margin-right: 0.5rem;

								&.mr-0 {
									margin-right: 0;
								}
							}

							@media screen and (max-width: (525px)) {
								font-size: 0.75rem;
							}
							@media screen and (max-width: (453px)) {
								font-size: 0.65rem;
							}
							@media screen and (max-width: (404px)) {
								font-size: 0.5rem;
							}
						}
					}
				}

				&__terminal {
					padding-left: 1rem;
					display: flex;
					align-items: center;
					&__path {
						color: $text-body;
						width: 7.5rem;

						@media screen and (max-width: (525px)) {
							font-size: 0.75rem;
							width: 5.8rem;
						}

						@media screen and (max-width: (453px)) {
							font-size: 0.65rem;
							width: 5rem;
						}
						@media screen and (max-width: (404px)) {
							font-size: 0.5rem;
							width: 3.9rem;
						}
					}

					&__output {
						background-color: $text-body;
						width: 0.5rem;
						height: 1rem;
						animation: terminal_output 1.5s infinite;

						@media screen and (max-width: (525px)) {
							width: 0.45rem;
							height: 0.9rem;
						}

						@media screen and (max-width: (453px)) {
							width: 0.4rem;
							height: 0.8rem;
						}
						@media screen and (max-width: (404px)) {
							width: 0.3rem;
							height: 0.6rem;
						}
					}
				}
			}
		}
	}

	@keyframes terminal_output {
		0% {
			opacity: 1;
		}
		50% {
			opacity: 0;
		}
		100% {
			opacity: 1;
		}
	}
</style>
