<script>
	const jobs = [
		{
			where: 'Kiiwa',
			what: 'Managing Director',
			when: 'March 2021 - Present'
		},

		{
			where: 'SLTec',
			what: 'Security Engineer',
			when: 'January 2020 - Present'
		},

		{
			where: 'Zero 7',
			what: 'Consulting Technical Manager',
			when: 'January 2020 - December 2021'
		},

		{
			where: 'Monzo',
			what: 'Financial Crime Specialist',
			when: 'January 2019 - December 2020'
		}
	];
</script>

<svelte:head>
	<title>Nathan Lindsay</title>
</svelte:head>

<div class="p-6">
	<div class="mx-auto max-w-lg space-y-6">
		<header class="space-y-6 text-center">
			<h1 class="text-xl font-medium">Nathan Lindsay</h1>

			<div>
				<p>I might do something with this website one day.</p>
				<p>Probably not though.</p>
			</div>
		</header>

		<main class="flex gap-6">
			<h2 class="flex-1 text-lg font-medium">Work</h2>
			<div class="space-y-6">
				{#each jobs as { where, what, when }}
					<div>
						<h3 class="font-medium">{where}</h3>
						<p>{what}</p>
						<p class="italic">{when}</p>
					</div>
				{/each}
			</div>
			<div class="flex-1" />
		</main>
	</div>
</div>
