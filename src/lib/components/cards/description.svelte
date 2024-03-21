<script lang="ts">
	export let items: string[];
</script>

<ul class="list">
	{#each items as item}
		<li><span class="flex-auto">{item}</span></li>
	{/each}
</ul>