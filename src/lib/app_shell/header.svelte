<script>
	import { AppBar, Avatar } from '@skeletonlabs/skeleton';
	import {
		InformationCircle,
		AcademicCap,
		Briefcase,
		CodeBracket
	} from '@inqling/svelte-icons/heroicon-24-outline';
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
		<div class="flex flex-row flex-wrap gap-4">
			<a class="btn btn-md variant-soft"
				 href="#about"
				 rel="noreferrer">
				<span><InformationCircle style="width: 24px;" /></span>
				<span>À propos</span>
			</a>
			<a class="btn btn-md variant-soft"
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

	</svelte:fragment>
</AppBar>
