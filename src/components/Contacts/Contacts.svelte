<script>
	import GitHub from "../Svg/GitHub.svelte";
	import GitLab from "../Svg/GitLab.svelte";
	import LinkedIn from "../Svg/LinkedIn.svelte";
	import Gmail from "../Svg/Gmail.svelte";
</script>

<nav>
	<div>
		<ul id="contacts">
			<li>
				<a
					href="https://github.com/angel-721"
					class="contrast"
					target="_blank"
					aria-label="Angel's github"
				>
					<GitHub size="2rem" fill="#dadedd" hoverFill="#fbfbfb" />
				</a>
			</li>
			<li>
				<a
					href="https://www.linkedin.com/in/angel-m-velasquez/"
					class="contrast"
					target="_blank"
					aria-label="Angel's Linkedin"
				>
					<LinkedIn size="2rem" fill="#dadedd" hoverFill="#fbfbfb" />
				</a>
			</li>
			<li>
				<a
					href="https://gitlab.com/angel-721"
					aria-label="Angel's Gitlab"
					class="contrast"
					target="_blank"
				>
					<GitLab size="2rem" fill="#dadedd" hoverFill="#fbfbfb" />
				</a>
			</li>
			<li>
				<a
					href="mailto:angelvelasquez2002@gmail.com"
					class="contrast"
					target="_blank"
					aria-label="Angel's Gmail"
				>
					<Gmail size="2rem" fill="#dadedd" hoverFill="#fbfbfb" />
				</a>
			</li>
		</ul>
	</div>
</nav>

<style lang="CSS">
	#contacts {
		margin-top: 12.5rem;
	}

	@media only screen and (max-width: 775px) {
		#contacts {
			margin-top: 2rem;
		}
	}
</style>
