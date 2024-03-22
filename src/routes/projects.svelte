<script>
	import { CodeBracket, ComputerDesktop, DevicePhoneMobile } from '@inqling/svelte-icons/heroicon-16-solid';
	import { Opensourceinitiative } from '@inqling/svelte-icons/simple-icons';

	import InfoLayout from '$lib/components/info_layout.svelte';
	import SectionCard from '$lib/components/cards/section_card.svelte';

	import IconLabel from '$lib/components/cards/icon_label.svelte';
	import IconButton from '$lib/components/cards/icon_button.svelte';
	import Description from '$lib/components/cards/description.svelte';
</script>

<span id="projects" />
<SectionCard>
	<h1 slot="title" class="h1">
		<span class="header-gradient from-orange-500 to-violet-500">Projets</span>
	</h1>
	<div slot="content" class="flex flex-col gap-8">
		<InfoLayout
			title="Material Notes">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconLabel label="Android">
					<DevicePhoneMobile style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Open source">
					<Opensourceinitiative style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="skills" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconLabel label="Flutter" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Dart" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Supabase" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Play Store" variant="variant-soft-primary">
					<ComputerDesktop style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description items={["Application Android de prise de notes réalisée avec Flutter"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4-4">
				<IconButton
					label="Play Store"
					url="https://play.google.com/store/apps/details?id=com.maelchiotti.localmaterialnotes/" />
				<IconButton
					label="GitHub"
					url="https://github.com/maelchiotti/LocalMaterialNotes/" />
			</div>
		</InfoLayout>

		<hr />

		<InfoLayout
			title="Cinema Project Manager">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconLabel label="Android, Windows, web">
					<DevicePhoneMobile style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Open source">
					<Opensourceinitiative style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="skills" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4-4">
				<IconLabel label="Flutter" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Dart" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label=".NET" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="C#" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="MongoDB" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Supabase" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Play Store" variant="variant-soft-primary">
					<ComputerDesktop style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description
					items={["Application multiplateformes de gestion de projet cinématographique réalisée avec Flutter et Supabase"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconButton
					label="GitHub"
					url="https://github.com/studiorvandco/cpm_app/" />
				<IconButton
					label="Studio Rv & Co"
					url="https://linktr.ee/studiorvandco" />
			</div>
		</InfoLayout>
	</div>
</SectionCard>
