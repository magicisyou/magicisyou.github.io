<script>
	import Repository from '../../components/organisms/Repository.svelte';
	const gh_base_link = 'https://github.com/magicisyou/';
	const gh_image_base = 'https://raw.githubusercontent.com/magicisyou/';
	const repos = [
		{
			name: 'Sudoku',
			description: 'Sudoku built with svelte and tauri',
			src: `${gh_base_link}sudoku`,
			image_url: `${gh_image_base}sudoku/main/docs/screenshot.webp`
		},
		{
			name: 'Easy Markdown',
			description: 'Markdown viewer and editor written in python',
			src: `${gh_base_link}easy-markdown`,
			image_url: `${gh_image_base}easy-markdown/main/docs/screenshot1.webp`
		},
		{
			name: 'Quick List',
			description: 'To do list app built with tauri',
			src: `${gh_base_link}quicklist`,
			image_url: `${gh_image_base}quicklist/main/docs/screenshot.webp`
		},
		{
			name: 'Fsearch',
			description: 'File content search tool',
			src: `${gh_base_link}fsearch`,
			image_url: `${gh_image_base}fsearch/main/docs/screenshot.webp`
		},
		{
			name: 'Termux Theme Changer',
			description: 'A shell script to change the theme of termux app',
			src: `${gh_base_link}termux-theme-changer`
		},
		{
			name: 'Repo Info',
			description:
				'Cli line tool written in rust to see the details of a github repository and to see the statistics of programming languages used',
			src: `${gh_base_link}repo-info`,
			image_url: `${gh_image_base}repo-info/main/docs/screenshot.webp`
		},
		{
			name: 'HCJ Lab',
			description:
				'Tauri app to write and previw HTML, CSS and Javascript code snippets instatntly',
			src: `${gh_base_link}hcj-lab`,
			image_url: `${gh_image_base}hcj-lab/main/docs/screenshot1.webp`
		},
		{
			name: 'IP Fetch',
			description:
				'Get geographical details of an ip address and print the location on a world map in the terminal',
			src: `${gh_base_link}ip-fetch`,
			image_url: `${gh_image_base}ip-fetch/main/docs/screenshot.webp`
		},
		{
			name: 'GVADER',
			description: 'GUI for VADER sentiment analysis',
			src: `${gh_base_link}gvader`,
			image_url: `${gh_image_base}gvader/main/docs/screenshot.webp`
		},
		{
			name: 'Color Palette',
			description: 'Tauri app to create personal color palette',
			src: `${gh_base_link}color-palette`,
			image_url: `${gh_image_base}color-palette/main/docs/screenshot.webp`
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
			image_url: `${gh_image_base}game-2048/main/docs/screenshot.webp`
		},
		{
			name: 'Calander',
			description: 'Calander for terminal written in rust',
			src: `${gh_base_link}calander`,
			image_url: `${gh_image_base}calander/main/docs/screenshot.webp`
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
