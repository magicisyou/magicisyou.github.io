<nav>
	<ul>
		<li>
			<a href="/">Home</a>
		</li>
		<li>
			<a href="/repositories">Repositories</a>
		</li>
	</ul>
</nav>

<style lang="scss">
	@import '../../styles/variables.scss';

	nav {
		height: 100%;

		ul {
			display: flex;
			flex-direction: row;
			height: inherit;

			li {
				display: inherit;
				align-items: center;

				a {
					display: flex;
					flex-direction: column;
					justify-content: center;
					padding: 0 1rem;
					height: 100%;
					width: 100%;
					color: inherit;
					text-transform: uppercase;
					text-decoration: none;
					text-align: center;
					transition: color 0.5s;

					&:hover {
						color: #f6f6f6;
					}
				}
			}
		}
	}
</style>
