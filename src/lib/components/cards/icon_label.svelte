<script lang="ts">
	export let label: string;
	export let variant: string = 'variant-soft';
</script>

<div class="badge {variant}">
	<div class="flex flex-row flex-center gap-1.5">
		<slot name="icon" />
		<p>{label}</p>
	</div>
</div>
