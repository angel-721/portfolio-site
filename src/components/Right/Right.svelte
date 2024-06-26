<script>
	import Experience from "../Experience/Experience.svelte";
	import AllProjects from "../AllProjcts/AllProjects.svelte";
</script>

<div class="container">
	<span class="fake-header">About</span>
	<div id="about">
		<p>
			I'm a first-year M.Eng. student at Lehigh University. I have a
			strong passion for Machine Learning and classical methods to extract
			meaning from data.
		</p>

		<p>
			I currently work as a VR Software Engineer for <a
				href="https://online.utahtech.edu/immersive/"
				target="_blank">Utah Tech Online</a
			>. Also, I teach
			<a href="https://computing.utahtech.edu/codeschool/" target="_blank"
				>Code School</a
			>, a 9-week full stack development course.
		</p>
		<p>
			When I'm not programming, I like to lift weights, go on runs, train
			in martial arts, and listen to 80's music! I'm a sports analytics
			nerd to make up for my horrible predictions.
		</p>
	</div>

	<span class="fake-header">Experience</span>
	<Experience />

	<span class="fake-header">Projects</span>
	<AllProjects />
</div>

<style lang="CSS">
	#about {
		padding-top: 3.5rem;
	}
	a {
		color: #e95b5b;
		text-decoration: none;
		font-weight: 500;
	}
	a:hover {
		color: lightcoral;
		cursor: pointer;
	}
	.fake-header {
		display: none;
		font-size: 1.2rem;
	}

	@media only screen and (max-width: 775px) {
		.fake-header {
			display: block;
			margin-bottom: -0.5rem;
			margin-top: 2.3rem;
		}
	}
</style>
