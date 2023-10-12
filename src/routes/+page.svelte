<script type="ts">
	import Note from '../components/molecules/Note.svelte';
	const notes = [
		{
			quote: 'Why I love thee? Ask why the seawind wanders, Why the shore is aflush with the tide',
			remarks:
				'This one of my favorite lines. It is the part of a poem written by Carl Sadakichi Hartmann.'
		},
		{
			quote:
				"You have been my friend. That in itself is a tremendous thing. I wove my webs for you because I liked you. After all, what's a life, anyway? We're born, we live a little while, we die. A spider's life can't help being something of a mess, with all this trapping and eating flies. By helping you, perhaps I was trying to lift up my life a trifle. Heaven knows anyone's life can stand a little of that.",
			remarks:
				"These lines are from the novel Charlotte's Web written by E.B White. Even though it's a children's novel it is a masterpiece. And these lines brought me to read the book which tells the story of friendship between Charlotte and Wilbur."
		}
	];
</script>

<h1>Magic Is You | You Are Magic</h1>
<p>I don't like to publish any personal details. So, Nothing to write.</p>
<div>
	{#each notes as note}
		<Note {...note} />
	{/each}
</div>

<style lang="scss" scoped>
	div {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: flex-start;
		gap: 20px;
		margin-top: 20px;
	}
</style>
