<script>
	import { AppBar, Avatar } from '@skeletonlabs/skeleton';
	import {
		InformationCircle,
		AcademicCap,
		Briefcase,
		CodeBracket,
		DocumentText
	} from '@inqling/svelte-icons/heroicon-24-outline';
</script>

<AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
	<svelte:fragment slot="lead">
		<a
			href="/"
			rel="noreferrer">
			<Avatar src="/assets/avatar.png" width="w-16" rounded="rounded-full" />
		</a>
	</svelte:fragment>

	<svelte:fragment>
		<a class="btn btn-md variant-soft"
			 href="#about"
			 rel="noreferrer">
			<span><InformationCircle class="icon" style="width:24px;" /></span>
			<span>À propos</span>
		</a>
		<a class="btn btn-md variant-soft"
			 href="#education"
			 rel="noreferrer">
			<span><AcademicCap class="icon" style="width:24px;" /></span>
			<span>Formation</span>
		</a>
		<a class="btn btn-md variant-soft"
			 href="#experiences"
			 rel="noreferrer">
			<span><Briefcase class="icon" style="width:24px;" /></span>
			<span>Expériences</span>
		</a>
		<a class="btn btn-md variant-soft"
			 href="#projects"
			 rel="noreferrer">
			<span><CodeBracket class="icon" style="width:24px;" /></span>
			<span>Projets</span>
		</a>
	</svelte:fragment>

	<svelte:fragment slot="trail">
		<a class="btn btn-md variant-soft-primary"
			 href="/assets/cv_fr.pdf"
			 target="_blank"
			 rel="noreferrer">
			<span><DocumentText class="icon" style="width:24px;" />
			</span><span>CV</span>
		</a>
	</svelte:fragment>
</AppBar>