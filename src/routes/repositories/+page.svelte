<script>
	import Repository from '../../components/organisms/Repository.svelte';
	const gh_base_link = 'https://github.com/youaremagic/';
	const repos = [
		{
			name: 'Termux Theme Changer',
			description: 'A shell script to change the theme of termux app',
			src: `${gh_base_link}termux-theme-changer`
		},
		{
			name: 'Repo Lang Stat',
			description:
				'Small cli line tool written in rust to get the statistics of programming languages used in a github repository',
			src: `${gh_base_link}repo-lang-stat`
		},
		{
			name: 'HCJ Lab',
			description:
				'Tauri app to write and previw HTML, CSS and Javascript code snippets instatntly',
			src: `${gh_base_link}hcj-lab`
		},
		{
			name: 'IP Fetch',
			description:
				'Get geographical details of an ip address and print the location on a world map in the terminal',
			src: `${gh_base_link}ip-fetch`
		},
		{
			name: 'Color Palette',
			description: 'Tauri app to create personal color palette',
			src: `${gh_base_link}color-palette`
		},
		{
			name: 'Color Game',
			description: 'A web game',
			src: `${gh_base_link}color-game`
		},
		{
			name: 'Game 2048',
			description: '2048 game built with tauri',
			src: `${gh_base_link}game-2048`
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
