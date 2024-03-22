<script>
	import { EnvelopeOpen } from '@inqling/svelte-icons/heroicon-24-solid';
	import { Github, Linkedin, Linktree } from '@inqling/svelte-icons/simple-icons';
</script>

<div class="flex-row gap-4">
	<a class="btn-icon variant-soft"
		 href="mailto:contact@maelchiotti.dev"
		 target="_blank"
		 rel="noreferrer">
		<EnvelopeOpen style="width: 24px;" />
	</a>
	<a class="btn-icon variant-soft"
		 href="https://linkstack.maelchiotti.dev/"
		 target="_blank"
		 rel="noreferrer">
		<Linktree style="width: 24px;" />
	</a>
	<a class="btn-icon variant-soft"
		 href="https://github.com/maelchiotti/"
		 target="_blank"
		 rel="noreferrer">
		<Github style="width: 24px;" />
	</a>
	<a class="btn-icon variant-soft"
		 href="https://www.linkedin.com/in/maelchiotti/"
		 target="_blank"
		 rel="noreferrer">
		<Linkedin style="width: 24px;" />
	</a>
</div>