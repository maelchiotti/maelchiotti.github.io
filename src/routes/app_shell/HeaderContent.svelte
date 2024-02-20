<script>
	import { ActionIcon, Center, Flex, Text, ThemeIcon } from '@svelteuidev/core';
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
		<Text variant='link' root='a' href='CV_-_Maël_Chiotti_-_FR.pdf'>CV</Text>
		<Text variant='link' root='a' href='#about'>À propos</Text>
		<Text variant='link' root='a' href='#experiences'>Expériences</Text>
		<Text variant='link' root='a' href='#training'>Formation</Text>
		<Text variant='link' root='a' href='#projects'>Projets</Text>
		<ActionIcon on:click={toggleTheme}>
			<ThemeIcon>
				<ThemeLightDark size="32" />
			</ThemeIcon>
		</ActionIcon>
	</Center>
</Flex>