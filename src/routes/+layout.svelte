<script lang="ts">
	import '../app.postcss';
	import '../app.css';

	import { AppShell } from '@skeletonlabs/skeleton';
	import Header from './app_shell/header.svelte';
	import Footer from './app_shell/footer.svelte';
</script>

<AppShell>
	<svelte:fragment slot="pageHeader">
		<Header></Header>
	</svelte:fragment>

	<slot />

	<svelte:fragment slot="pageFooter">
		<Footer></Footer>
	</svelte:fragment>
</AppShell>
