<script lang="ts">
	export let title: string;
	export let content: string;
	export let badges: string[];
</script>

<div class="card card-hover size-33-percents p-4 variant-glass-surface">
	<div class="flexbox-column flexbox-center">
		<header class="card-header">
			<h3 class="h3">{title}</h3></header>
		<section class="p-4">
			<p>{content}</p></section>
		<footer class="card-footer">
			<div class="flexbox-row flexbox-center">
				{#each badges as badge}
					<p class="badge variant-filled">{badge}</p>
				{/each}
			</div>
		</footer>
	</div>
</div>