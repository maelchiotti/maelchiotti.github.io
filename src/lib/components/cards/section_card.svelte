<div class="card card-hover card-size variant-glass-surface p-12">
	<div class="flex flex-col flex-center gap-16">
		<header class="card-header">
			<slot name="title" />
		</header>
		<section>
			<slot name="content" />
		</section>
	</div>
</div>

<style>
    .card-size {
        width: 50%;
        min-width: 512px;
        max-width: 1024px;
    }
</style>