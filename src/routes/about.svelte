<script>
	import { ArrowDown } from '@inqling/svelte-icons/heroicon-24-solid';
	import { Github, Linkedin, Linktree } from '@inqling/svelte-icons/simple-icons';
</script>

<div class="full-height flex flex-col flex-evenly">
	<div class="flex flex-col flex-center gap-4">
		<h1 class="h1 jet-brains-mono">Maël Chiotti</h1>
		<h3 class="h3 jet-brains-mono">Développeur full-stack et vice-président du Studio Rv & Co</h3>
		<div class="flex flex-row flex-wrap gap-4 p-8">
			<a class="btn btn-xl variant-ghost-primary"
				 href="https://linkstack.maelchiotti.dev/"
				 target="_blank"
				 rel="noreferrer">
				<span><Linktree style="width: 24px;" /></span>
				<span>LinkStack</span>
			</a>
			<a class="btn btn-xl variant-ghost-primary"
				 href="https://github.com/maelchiotti/"
				 target="_blank"
				 rel="noreferrer">
				<span><Github style="width: 24px;" /></span>
				<span>GitHub</span>
			</a>
			<a class="btn btn-xl variant-ghost-primary"
				 href="https://www.linkedin.com/in/maelchiotti/"
				 target="_blank"
				 rel="noreferrer">
				<span><Linkedin style="width: 24px;" /></span>
				<span>LinkedIn</span>
			</a>
		</div>
	</div>
	<div>
		<a class="btn-icon variant-filled bounce"
			 href="#education"
			 rel="noreferrer">
			<ArrowDown style="width: 24px;" />
		</a>
	</div>
</div>

<style>
    .full-height {
        height: 100vh;
        min-height: 256px;
    }
</style>