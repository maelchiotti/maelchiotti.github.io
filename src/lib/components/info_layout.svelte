<script lang="ts">
	export let title: string;
</script>

<div class="flex flex-col flex-center">
	<header>
		<h3 class="h3">{title}</h3>
	</header>
	<section class="pb-4 pt-4">
		<div class="flex flex-col flex-wrap flex-center gap-4">
			<slot name="badges" />
			<slot name="skills" />
			<slot name="content" />
		</div>
	</section>
	<footer>
		<slot name="footer" />
	</footer>
</div>
