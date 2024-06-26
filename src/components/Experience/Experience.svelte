<script>
	import Education from "../Education/Education.svelte";
	import WorkPlace from "../WorkPlace/WorkPlace.svelte";

	let utahTechBio = [
		"Conducted research MVA on southern Utah water quality with principal component analysis",
		"Various of web applications and machine-learning projects for my coursework",
		"Graduated with Magna Cum Laude Latin honors",
	];

	let UTSkills = ["C#", "Unity", "SCM"];

	let CodeSchoolSkills = [
		"JavaScript",
		"Express.js",
		"MongoDB",
		"Node.js",
		"Vue.js",
		"Git",
	];
	let codeSchoolPoints = [
		"Teach students full stack web development",
		"Introduce software practices such as version control via Git",
	];
	let UtOnlinePoints = [
		"Design and develop virtual reality classroom experiences for Utah Tech Online",
		"Optimize existing systems while using networking APIs to synchronize for all clients",
		"Document the systems I create for future engineers",
	];
</script>

<div class="container" id="experience">
	<a id="resume-link" href="assets/resume.pdf" target="_blank">
		<div id="resume">
			<span id="resume-text">Check Out My Full Resume</span>
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
	<Education
		school="Utah Tech University"
		degree="B.S."
		major="Software Engineering"
		startYear="2022"
		endYear="2024"
		bio={utahTechBio}
		gpa="3.91"
	/>

	<WorkPlace
		company="Utah Tech University"
		role="Code School Instructor"
		startYear="2024"
		endYear="present"
		skills={CodeSchoolSkills}
		points={codeSchoolPoints}
	/>

	<WorkPlace
		company="Utah Tech Online"
		role="VR Software Engineer"
		startYear="2023"
		endYear="present"
		points={UtOnlinePoints}
		skills={UTSkills}
	/>
</div>

<style lang="CSS">
	#experience {
		margin-top: 3rem;
		padding-top: 0.3rem;
	}
	#resume-text {
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
	a {
		text-decoration: none;
		font-weight: 500;
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
		#experience {
			padding-left: 0;
		}
	}
</style>
