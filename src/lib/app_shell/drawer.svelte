<script lang="ts">
	import SocialLinks from '$lib/app_shell/social_links.svelte';
	import { AcademicCap, Briefcase, CodeBracket } from '@inqling/svelte-icons/heroicon-24-outline';
	import { Drawer, getDrawerStore } from '@skeletonlabs/skeleton';

	const drawerStore = getDrawerStore();

	function drawerClose(): void {
		drawerStore.close();
	}
</script>

<Drawer>
	<div class="flex flex-col justify-stretch" style="height: 100%">
		<nav class="flex-grow list-nav p-4">
			<a class="btn btn-md variant-soft mb-2.5"
				 href="#education"
				 rel="noreferrer"
				 on:click={drawerClose}>
				<span><AcademicCap style="width: 24px;" /></span>
				<span>Formation</span>
			</a>
			<a class="btn btn-md variant-soft mb-2.5"
				 href="#experiences"
				 rel="noreferrer"
				 on:click={drawerClose}>
				<span><Briefcase style="width: 24px;" /></span>
				<span>Expériences</span>
			</a>
			<a class="btn btn-md variant-soft mb-2.5"
				 href="#projects"
				 rel="noreferrer"
				 on:click={drawerClose}>
				<span><CodeBracket style="width: 24px;" /></span>
				<span>Projets</span>
			</a>
		</nav>

		<div class="flex flex-center mb-2.5">
			<SocialLinks />
		</div>
	</div>
</Drawer>
