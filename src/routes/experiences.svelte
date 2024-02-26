<script>
	import { MapPin, Calendar, Clock, ComputerDesktop, CodeBracket } from '@inqling/svelte-icons/heroicon-16-solid';

	import InfoLayout from '$lib/components/info_layout.svelte';
	import SectionCard from '$lib/components/cards/section_card.svelte';

	import IconLabel from '$lib/components/cards/icon_label.svelte';
	import IconButton from '$lib/components/cards/icon_button.svelte';
	import Description from '$lib/components/cards/description.svelte';
</script>

<span id="experiences" />
<SectionCard>
	<h1 slot="title" class="h1">
		<span class="header-gradient from-orange-500 to-violet-500">Expériences</span>
	</h1>
	<div slot="content" class="flex flex-col gap-8">
		<InfoLayout
			title="Développement mobile full-stack">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-4">
				<IconLabel label="Qim info">
					<MapPin style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="2023">
					<Calendar style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="6 mois">
					<Clock style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="skills" class="flex flex-row flex-wrap flex-center gap-4">
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
				<IconLabel label="fastlane" variant="variant-soft-primary">
					<ComputerDesktop style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Play Store" variant="variant-soft-primary">
					<ComputerDesktop style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description items={[
					"Développement en Flutter d'une application mobile interne à destination des employés",
					"Développement en .NET d'une API permettant à l'application d'interagir avec les différents services de l'entreprise",
					"Mise en application du framework agile Scrum"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-4">
				<IconButton label="Qim info" url="https://www.qiminfo.ch/" />
			</div>
		</InfoLayout>

		<hr />

		<InfoLayout
			title="Développement logiciel front-end">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-4">
				<IconLabel label="LERTI">
					<MapPin style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="2022">
					<Calendar style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="6 mois">
					<Clock style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="skills" class="flex flex-row flex-wrap flex-center gap-4">
				<IconLabel label="Python" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="PyQt" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description items={[
					"Développement en Python d'un logiciel de traitement de données",
					"Conception d'interfaces utilisateur avec Qt",
					"Support logiciel et suivi de l'expérience utilisateur"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-4">
				<IconButton label="LERTI" url="https://www.lerti.fr/" />
			</div>
		</InfoLayout>

		<hr />

		<InfoLayout
			title="Développement et traitement de données">
			<div slot="badges" class="flex flex-row flex-wrap flex-center gap-4">
				<IconLabel label="INRAE">
					<MapPin style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="2020">
					<Calendar style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="3 mois">
					<Clock style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="skills" class="flex flex-row flex-wrap flex-center gap-4">
				<IconLabel label="C" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Scala" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
				<IconLabel label="Java" variant="variant-soft-primary">
					<CodeBracket style="width: 20px;" slot="icon" />
				</IconLabel>
			</div>
			<div slot="content">
				<Description items={[
					"Analyse de banques de données génétiques",
					"Développement d’algorithmes en Scala pour Apache Spark",
					"Étude de solutions pour l'exécution de code en C dans Spark"]} />
			</div>
			<div slot="footer" class="flex flex-row flex-wrap flex-center gap-4">
				<IconButton label="INRAE" url="https://www.inrae.fr/" />
				<IconButton label="LIPME" url="https://www.lipme.fr/" />
			</div>
		</InfoLayout>
	</div>
</SectionCard>
