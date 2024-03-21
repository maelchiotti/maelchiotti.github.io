<script lang="ts">
	import '../app.postcss';
	import '../app.css';

	import { AppShell, initializeStores } from '@skeletonlabs/skeleton';
	import Header from '$lib/app_shell/header.svelte';
	import Footer from '$lib/app_shell/footer.svelte';
	import Drawer from '$lib/app_shell/drawer.svelte';

	initializeStores();
</script>

<Drawer />

<AppShell>
	<svelte:fragment slot="pageHeader">
		<Header />
	</svelte:fragment>

	<slot />

	<svelte:fragment slot="pageFooter">
		<Footer />
	</svelte:fragment>
</AppShell>
