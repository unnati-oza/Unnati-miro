<script>
	import Note from '../Note.svelte';
	
	let notes = [
		{
			id: 1,
			text: 'Enter Text here'
		},
		{
			id: 2,
			text: 'Enter Text here'
		}
	];
</script>

{#each notes as note}
	<Note>
		<div contenteditable>{note.text}</div>
	</Note>
{/each}

<style>
	div {
		background: lightcoral;
		padding: 20px;
		width: 350px;
		text-align: center;
	}
</style>