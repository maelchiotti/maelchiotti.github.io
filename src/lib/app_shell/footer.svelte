<script>
	import { AppBar, LightSwitch } from '@skeletonlabs/skeleton';
	import { Github, Linkedin, Linktree } from '@inqling/svelte-icons/simple-icons';
	import { AtSymbol } from '@inqling/svelte-icons/heroicon-24-solid';
</script>

<AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
	<svelte:fragment slot="lead">
		<LightSwitch></LightSwitch>
	</svelte:fragment>

	<svelte:fragment>
		Fait avec ❤️ par Maël Chiotti
	</svelte:fragment>

	<svelte:fragment slot="trail">
		<a class="btn-icon variant-soft"
			 href="mailto:contact@maelchiotti.dev"
			 target="_blank"
			 rel="noreferrer">
			<AtSymbol style="width: 24px;" />
		</a>
		<a class="btn-icon variant-soft"
			 href="https://linkstack.maelchiotti.dev/"
			 target="_blank"
			 rel="noreferrer">
			<Linktree style="width: 24px;" />
		</a>
		<a class="btn-icon variant-soft"
			 href="https://github.com/maelchiotti/"
			 target="_blank"
			 rel="noreferrer">
			<Github style="width: 24px;" />
		</a>
		<a class="btn-icon variant-soft"
			 href="https://www.linkedin.com/in/maelchiotti/"
			 target="_blank"
			 rel="noreferrer">
			<Linkedin style="width: 24px;" />
		</a>
	</svelte:fragment>
</AppBar>