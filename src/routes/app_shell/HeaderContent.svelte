<script>
	import { ActionIcon, Center, Flex } from '@svelteuidev/core';
	import ThemeLightDark from 'svelte-material-icons/ThemeLightDark.svelte';
	import { createEventDispatcher } from 'svelte';

	const toggleThemeEvent = createEventDispatcher();

	function toggleTheme() {
		toggleThemeEvent('toggleTheme');
	}
</script>

<Flex justify="space-between">
	<h1>Maël Chiotti</h1>
	<Center>
		<ActionIcon on:click={toggleTheme}>
			<ThemeLightDark size="32" />
		</ActionIcon>
	</Center>
</Flex>