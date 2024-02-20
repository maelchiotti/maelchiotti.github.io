<script lang="ts">
	import '@fontsource-variable/montserrat';

	import { Footer, SvelteUIProvider } from '@svelteuidev/core';
	import { AppShell, Header } from '@svelteuidev/core';

	import HeaderContent from './app_shell/HeaderContent.svelte';
	import FooterContent from './app_shell/FooterContent.svelte';

	let darkTheme = true;
</script>

<style>
    :global(body) {
        font-family: "Montserrat Variable", sans-serif;
    }
</style>

<SvelteUIProvider withNormalizeCSS withGlobalStyles themeObserver={darkTheme ? 'dark' : 'light'}>
	<AppShell fixed>
		<Header fixed slot="header" height="100">
			<HeaderContent on:toggleTheme={()=>darkTheme=!darkTheme} />
		</Header>

		<slot />

		<Footer slot="footer" height="100">
			<FooterContent />
		</Footer>
	</AppShell>
</SvelteUIProvider>