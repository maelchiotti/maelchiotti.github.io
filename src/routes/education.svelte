<script>
	import { Calendar, MapPin } from '@inqling/svelte-icons/heroicon-16-solid';

	import InfoLayout from '$lib/components/info_layout.svelte';
	import SectionCard from '$lib/components/cards/section_card.svelte';

	import IconLabel from '$lib/components/cards/icon_label.svelte';
	import IconButton from '$lib/components/cards/icon_button.svelte';
	import Description from '$lib/components/cards/description.svelte';
</script>

<span id="education" />
<SectionCard>
	<h1 slot="title" class="h1">
		<span class="header-gradient from-orange-500 to-violet-500">Formation</span>
	</h1>
	<div slot="content" class="flex flex-col gap-8">
		<InfoLayout
			title="Diplôme d'ingénieur en informatique">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconLabel label="Grenoble">
					<MapPin style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="2023">
					<Calendar style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description items={[
					"Polytech Grenoble - INP - Université Grenoble Alpes",
					"Spécialité Communication Multimédia"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconButton label="Polytech Grenoble" url="https://polytech.grenoble-inp.fr/" />
			</div>
		</InfoLayout>
		<hr />
		<InfoLayout
			title="Diplôme Universitaire Technologique en informatique">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconLabel label="Toulouse">
					<MapPin style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="2020">
					<Calendar style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description items={["IUT de l'université Toulouse III"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-x-2 gap-y-2 md:gap-x-4">
				<IconButton label="IUT Paul Sabatier" url="https://iut.univ-tlse3.fr/" />
			</div>
		</InfoLayout>
	</div>
</SectionCard>
