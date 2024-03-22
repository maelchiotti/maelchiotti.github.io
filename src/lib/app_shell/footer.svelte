<script>
	import SocialLinks from '$lib/app_shell/social_links.svelte';
	import { AppBar, LightSwitch } from '@skeletonlabs/skeleton';
</script>

<AppBar gridColumns="1">
	<div class="flex flex-col flex-center justify-between gap-4 md:flex-row">
		<LightSwitch></LightSwitch>

		<div class="flex-center flex-grow">
			Fait avec ❤️ par Maël Chiotti
		</div>

		<SocialLinks />
	</div>

</AppBar>