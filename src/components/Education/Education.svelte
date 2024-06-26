<script>
	export let school;
	export let degree;
	export let major;
	export let startYear;
	export let endYear;
	export let bio;
	export let gpa;
</script>

<div class="grid ed-content">
	<div class="main-ed">
		<p style="font-size: 1.4rem;">{school}</p>
		<p style="font-size: 0.75rem; margin-top:-0.8rem">
			{degree}
			{major}
			&#8213; GPA: {gpa}
		</p>
		<ul class="bio">
			{#each bio as point}
				<li style=" list-style-type:circle;">
					{point}
				</li>
			{/each}
		</ul>
	</div>
	<div id="date">
		{startYear} &#8213; {endYear}
	</div>
</div>

<style lang="CSS">
	.bio {
		font-size: 0.9rem;
	}
	#date {
		padding-top: 0.1rem;
		font-size: 0.8rem;
		grid-column: 6/8;
	}

	.main-ed {
		grid-column: 1/6;
	}

	.ed-content {
		margin-top: 3rem;
		margin-bottom: 2rem;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(7, 1fr);
	}
	@media only screen and (max-width: 775px) {
		.grid {
			display: grid;
			grid-template-rows: repeat(7, 1fr);
		}
		#date {
			padding-top: 0.1rem;
			font-size: 0.8rem;
			grid-row: 1/1;
			grid-column: 1/-1;
		}

		.main-ed {
			grid-row: 1/7;
			grid-column: 1/-1;
			margin-top: 1.5rem;
		}
	}
</style>
