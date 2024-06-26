<script>
	export let company;
	export let role;
	export let startYear;
	export let endYear;
	export let skills;
	export let points;
</script>

<div class="grid ed-content">
	<div class="main-ed">
		<p style="font-size: 1.3rem;">{role}</p>
		<p style="font-size: 0.75rem; margin-top:-0.8rem">
			{company}
		</p>
		<ul class="bio">
			{#each points as point}
				<li style=" list-style-type: disc;">
					{point}
				</li>
			{/each}
		</ul>

		<ul class="skills">
			{#each skills as skill}
				<li class="skill-tag">
					{skill}
				</li>
			{/each}
		</ul>
	</div>
	<div id="date">
		{startYear} - {endYear}
	</div>
</div>

<style lang="CSS">
	.skills {
		padding: 0;
	}
	.skill-tag {
		display: inline-block;
		list-style: none;
		background: lightcoral;
		border-radius: 14px;
		padding: 5px 10px;
		font-size: 0.75rem;
		color: black;
		margin-right: 0.5rem;
		margin-bottom: 0.5rem;
	}
	.bio {
		font-size: 0.9rem;
		margin-bottom: 1.2rem;
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
