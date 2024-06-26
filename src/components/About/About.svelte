<script>
	import Education from "../Education/Education.svelte";
</script>

<div>
	<h2 style="text-align: center;">Education:</h2>

	<Education
		school={"Utah Tech University"}
		degree={"Bachelor of Science"}
		major={"Software Engineering"}
		gpa={3.91}
		startYear={2022}
		endYear={2024}
	/>
</div>

<style lang="CSS">
	div {
		margin-top: 2rem;
	}
</style>
