<script>
	import Project from "../Project/Project.svelte";
	import lyric_luminary from "../../../public/assets/images/lyric.webp";
	import godot_class from "../../../public/assets/images/cat.webp";
	import ufp from "../../../public/assets/images/ufp.webp";

	const lyric_bio =
		"This is a fun project that aims to view lyrics via the lens of a text classification model. I'm experimenting with TF-IDF to classify songs into a genere via the lyrics of the song.";
	const godot_bio =
		"Use a pre-trained convolutional neural network to make in game predictions! Take screenshots of the game and classify if a cat or dog is in the scene with the power of machine learning.";
	const ufp_bio =
		"A web app that allows users to predict the outcome of mixed martial arts bouts. I created a machine learning model to predict MMA bouts and incorporated into this front end!";
</script>

<div id="projects">
	<Project
		name="Lyric-Luminary"
		bio={lyric_bio}
		image={lyric_luminary.src}
		img_alt="Lyric Luminary"
		link="https://github.com/angel-721/lyric-luminary"
	/>
	<Project
		name="Godot Image Classification "
		bio={godot_bio}
		image={godot_class.src}
		img_alt="Godot Image Classification"
		link="https://github.com/angel-721/godot-image-classification"
	/>
	<Project
		name="Ultimate Fight Predictor"
		bio={ufp_bio}
		image={ufp.src}
		img_alt="Ultimate Fight Predictor"
		link="https://github.com/angel-721/ultimate-fight-predictor"
	/>
</div>
<a id="project-link" href="/projects">
	<div id="projectz">
		<span id="project-text">Repository For All Projects</span>
		<svg
			xmlns="http://www.w3.org/2000/svg"
			height="24px"
			viewBox="0 -960 960 960"
			width="24px"
			fill="currentColor"
			><path
				d="m560-240-56-58 142-142H160v-80h486L504-662l56-58 240 240-240 240Z"
			/></svg
		>
	</div>
</a>

<style lang="CSS">
	#projectz {
		margin-top: 2rem;
	}
	#project-text {
		color: white;
		font-weight: 500;
	}
	a svg {
		color: white;
		width: 30px;
		height: 30px;
	}
	a:hover svg {
		color: pink;
		animation: move-top-right 1s ease-in-out;
		animation-fill-mode: forwards;
	}
	a:hover span {
		text-decoration: underline;
		text-decoration-color: pink;
	}
	a {
		text-decoration: none;
		font-weight: 500;
	}

	#projects {
		margin-top: 3rem;
		padding-top: 2.8rem;
	}
	@keyframes move-top-right {
		0% {
			transform: translate(0, 0);
		}
		100% {
			transform: translate(5px);
		}
	}
	@media only screen and (max-width: 775px) {
		#projects {
			padding-left: 0;
		}
	}
</style>
