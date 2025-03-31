<script>
	/* Heading
	based on Kirby implementation
	https://getkirby.com/docs/reference/panel/blocks/heading
	
	*/

	export let block = {
		content: {
			level: "h2",
			text: ""
		},
		id: "",
		isHidden: true,
		type: "heading"
	};

	const { level, text } = block.content;
</script>

{#if !block.isHidden}
	<svelte:element this={level}>{text}</svelte:element>
{/if}
