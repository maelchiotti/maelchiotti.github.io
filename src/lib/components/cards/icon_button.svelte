<script lang="ts">
	import { Link } from '@inqling/svelte-icons/heroicon-16-solid';

	export let label: string;
	export let url: string;
</script>

<a class="btn btn-sm variant-ghost"
	 href={url}
	 target="_blank"
	 rel="noreferrer">
	<span><Link style="width: 20px;" /></span>
	<span>{label}</span>
</a>
