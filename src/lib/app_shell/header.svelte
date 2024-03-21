<script lang="ts">
	import { AppBar, Avatar, getDrawerStore } from '@skeletonlabs/skeleton';
	import { AcademicCap, Bars3, Briefcase, CodeBracket } from '@inqling/svelte-icons/heroicon-24-outline';

	const drawerStore = getDrawerStore();

	function drawerOpen(): void {
		drawerStore.open({
			position: 'right',
			width: 'w-[256px]',
			padding: 'p-4',
			rounded: 'rounded-xl'
		});
	}
</script>

<AppBar>
	<svelte:fragment slot="lead">
		<a
			href="/"
			rel="noreferrer">
			<Avatar src="/assets/avatar.png" width="w-16" rounded="rounded-full" />
		</a>
	</svelte:fragment>

	<h3 class="h3">Bienvenue !</h3>

	<svelte:fragment slot="trail">
		<div class="flex-row flex-wrap justify-end gap-4 hidden md:flex">
			<a class="btn btn-md variant-soft "
				 href="#education"
				 rel="noreferrer">
				<span><AcademicCap style="width: 24px;" /></span>
				<span>Formation</span>
			</a>
			<a class="btn btn-md variant-soft"
				 href="#experiences"
				 rel="noreferrer">
				<span><Briefcase style="width: 24px;" /></span>
				<span>Expériences</span>
			</a>
			<a class="btn btn-md variant-soft"
				 href="#projects"
				 rel="noreferrer">
				<span><CodeBracket style="width: 24px;" /></span>
				<span>Projets</span>
			</a>
		</div>
		<button class="btn-icon variant-soft md:hidden" on:click={drawerOpen}>
			<Bars3 style="width: 24px;" />
		</button>

	</svelte:fragment>
</AppBar>
