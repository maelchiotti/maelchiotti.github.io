<script>
	import Hello from './hello.svelte';
	import Education from './education.svelte';
	import Experiences from './experiences.svelte';
	import Projects from './projects.svelte';
</script>

<div class="flex flex-col flex-center gap-16 p-32-bottom">
	<Hello />
	<Education />
	<Experiences />
	<Projects />
</div>

<style>
    .p-32-bottom {
        padding-bottom: 128px;
    }
</style>