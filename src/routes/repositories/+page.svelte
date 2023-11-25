<script>
	import Repository from '../../components/organisms/Repository.svelte';
	const gh_base_link = 'https://github.com/youaremagic/';
	const repos = [
		{
			name: 'Sudoku',
			description: 'Sudoku built with svelte and tauri',
			src: `${gh_base_link}sudoku`,
			image_url:'https://raw.githubusercontent.com/youaremagic/sudoku/main/docs/screenshot.webp',
		},
		{
			name: 'Termux Theme Changer',
			description: 'A shell script to change the theme of termux app',
			src: `${gh_base_link}termux-theme-changer`
		},
		{
			name: 'Repo Lang Stat',
			description:
				'Small cli line tool written in rust to get the statistics of programming languages used in a github repository',
			src: `${gh_base_link}repo-lang-stat`,
			image_url:'https://raw.githubusercontent.com/youaremagic/repo-lang-stat/main/docs/screenshot.webp',
		},
		{
			name: 'HCJ Lab',
			description:
				'Tauri app to write and previw HTML, CSS and Javascript code snippets instatntly',
			src: `${gh_base_link}hcj-lab`,
			image_url:'https://raw.githubusercontent.com/youaremagic/hcj-lab/main/docs/screenshot1.webp',
		},
		{
			name: 'IP Fetch',
			description:
				'Get geographical details of an ip address and print the location on a world map in the terminal',
			src: `${gh_base_link}ip-fetch`,
			image_url:'https://raw.githubusercontent.com/youaremagic/ip-fetch/main/docs/screenshot.webp',
		},
		{
			name: 'GVADER',
			description: 'GUI for VADER sentiment analysis',
			src: `${gh_base_link}gvader`,
			image_url:'https://raw.githubusercontent.com/youaremagic/gvader/main/docs/screenshot.webp',
		},
		{
			name: 'Color Palette',
			description: 'Tauri app to create personal color palette',
			src: `${gh_base_link}color-palette`,
			image_url:'https://raw.githubusercontent.com/youaremagic/color-palette/main/docs/screenshot.webp',
		},
		{
			name: 'Color Game',
			description: 'A web game',
			src: `${gh_base_link}colorgame`
		},
		{
			name: 'Game 2048',
			description: '2048 game built with tauri',
			src: `${gh_base_link}game-2048`,
			image_url:'https://raw.githubusercontent.com/youaremagic/game-2048/main/docs/screenshot.webp',
		}
	];
</script>

<div>
	{#each repos as repo}
		<Repository {...repo} />
	{/each}
</div>

<style lang="scss" scoped>
	div {
		display: flex;
		flex-direction: column;
		gap: 10px;
	}
</style>
