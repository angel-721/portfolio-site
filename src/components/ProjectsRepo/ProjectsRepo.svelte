<script>
	import ProjectRow from "../ProjectRow/ProjectRow.svelte";
</script>

<div id="all-projects" class="container">
	<h1>Project Repository</h1>
	<table>
		<thead>
			<tr>
				<th scope="col">Project</th>
				<th scope="col" id="company">Company</th>
				<th scope="col">Technologies</th>
				<th scope="col" id="link">Link</th>
			</tr>
		</thead>
		<tbody>
			<ProjectRow
				project_name="PHYSICS 2215"
				company="Utah Tech Online"
				technologies={["C#", "Unity", "Oculus"]}
				isGithub={false}
				link="https://www.youtube.com/watch?v=ead660LGiRM"
				url="Demo Video"
			/>
			<ProjectRow
				project_name="Personal Website"
				company=""
				technologies={["SvelteJS", "HTML", "CSS", "Astro"]}
				isGithub={false}
				link="/"
				url="amvelasquez.dev"
			/>
			<ProjectRow
				project_name="Lyric Luminary"
				company=""
				technologies={[
					"Python",
					"Go",
					"SvelteJS",
					"CSS",
					"Nim",
					"scikit-learn",
				]}
				isGithub={true}
				link="https://github.com/angel-721/lyric-luminary"
			/>
			<ProjectRow
				project_name="Multivariate analysis of southern Utah water quality"
				company="Utah Tech Research"
				technologies={["Python", "Jupyter", "scikit-learn"]}
				isGithub={true}
				link="https://github.com/angel-721/mva-of-southern-utah-water-quality/"
			/>
			<ProjectRow
				project_name="UFP"
				company=""
				technologies={["Python", "Pandas", "NumPy", "scikit-learn"]}
				isGithub={true}
				link="https://github.com/angel-721/ufp"
			/>
			<ProjectRow
				project_name="Ultimate Fight Predictor"
				company=""
				technologies={[
					"Vue.js",
					"HTML",
					"CSS",
					"Express.js",
					"MongoDB",
				]}
				isGithub={true}
				link="https://github.com/angel-721/ultimate-fight-predictor"
			/>
			<ProjectRow
				project_name="Tapology Python Parser"
				company=""
				technologies={["Python", "Beautiful Soup"]}
				isGithub={true}
				link="https://github.com/angel-721/tapology-python-parser/tree/main"
			/>
			<ProjectRow
				project_name="Tweepy Media Bot"
				company=""
				technologies={["Python", "SQL", "Twitter API", "AWS"]}
				isGithub={true}
				link="https://github.com/angel-721/tweepy-media-bot"
			/>
			<ProjectRow
				project_name="Godot(HTTP Client Unit Test)"
				company="Open Source Contribution"
				technologies={["C++"]}
				link="https://github.com/godotengine/godot/pull/76636"
				isGithub={true}
			/>
			<ProjectRow
				project_name="MyMood"
				company="Open Source Contribution"
				technologies={["Kotlin", "Android"]}
				link="https://github.com/NimaKhajehpour/MyMood/pull/19"
				isGithub={true}
			/>
			<ProjectRow
				project_name="NookBeats"
				company=""
				technologies={["Kotlin", "Android"]}
				link=""
			/>
			<ProjectRow
				project_name="MindJot"
				company=""
				technologies={[
					"Python",
					"Flask",
					"HTML",
					"CSS",
					"SQL",
					"JavaScript",
				]}
				link=""
			/>
			<ProjectRow
				project_name="Tuneleaf"
				company=""
				technologies={[
					"Python",
					"Flask",
					"HTML",
					"CSS",
					"SQL",
					"JavaScript",
				]}
				link=""
			/>
			<ProjectRow
				project_name="Image to Ascii Converter"
				company=""
				technologies={[
					"Java"
				]}
				link="https://github.com/angel-721/java-image-ascii-converter"
				isGithub={true}
			/>
			<ProjectRow
				project_name="Compubox Python"
				company=""
				technologies={["Python", "SQL"]}
				isGithub={true}
				link="https://github.com/angel-721/compubox-python"
			/>
		</tbody>
	</table>
</div>

<style>
	h1 {
		margin-bottom: 3rem;
	}
	#all-projects {
		margin-top: 1.5rem;
	}
	@media only screen and (max-width: 675px) {
		#company,
		#link {
			display: none;
		}
	}
</style>
