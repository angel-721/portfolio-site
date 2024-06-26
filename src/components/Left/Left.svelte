<script>
	import NavBar from "../NavBar/NavBar.svelte";
	import Contacts from "../Contacts/Contacts.svelte";
</script>

<div class="container" id="left-side">
	<div id="intro-header">
		<h1>Angel Velasquez</h1>
		<p>M.Eng Computer Science Student</p>
		<div id="intro">
			<p>Aspiring Machine Learning Engineer with a</p>
			<p>strong interest in web development.</p>
		</div>
	</div>
	<NavBar />
	<Contacts />
</div>

<style lang="CSS">
	#intro {
		margin-top: 2rem;
	}

	p {
		margin-top: -0.5rem;
	}

	#intro > p {
		margin-top: -0.8rem;
		color: #b3b3b3;
		font-size: 0.8rem;
	}
	#left-side {
		padding-top: 3rem;
	}
</style>
