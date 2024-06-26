<script>
	export let project_name;
	export let company;
	export let technologies;
	export let url;
	export let link;
	export let isGithub = false;
	import GitHub from "../Svg/GitHub.svelte";
</script>

<tr>
	<th scope="row" id="td-name">{project_name}</th>
	<th scope="row" id="td-name-mobile">
		<div>
			{#if link}
				<a href={link} class="contrast" target="_blank"
					>{project_name}

					<svg
						xmlns="http://www.w3.org/2000/svg"
						height="24px"
						viewBox="0 -960 960 960"
						width="24px"
						><path
							d="m560-240-56-58 142-142H160v-80h486L504-662l56-58 240 240-240 240Z"
						/></svg
					>
				</a>
			{:else}
				{project_name}
			{/if}
		</div>
	</th>
	<td id="td-company">{company}</td>
	<td id="td-tech">
		<ul class="skills">
			{#each technologies as skill}
				<li class="skill-tag">
					{skill}
				</li>
			{/each}
		</ul></td
	>
	{#if isGithub}
		<td id="link-td">
			<a href={link} class="contrast" target="_blank">
				Github
				<GitHub
					fill="currentColor;"
					hoverFill="currentColor"
					size="32px"
					mBottom="0.43rem"
				/>
			</a>
		</td>
	{:else if link != ""}
		<td id="link-td">
			<a
				href={link}
				target="_blank"
				class="contrast"
				style="text-decoration: underline; font-size: .93rem;">{url}</a
			>
		</td>
	{:else}
		<td id="link-td" />
	{/if}
</tr>

<style lang="CSS">
	#td-name {
		font-weight: 600;
		width: 10rem;
	}
	#td-company {
		width: 10rem;
		font-size: 0.85rem;
	}
	#link-td {
		width: 7rem;
	}
	#td-tech {
		width: 9rem;
	}
	.skills {
		padding-top: 1.5rem;
		padding-left: 0;
	}
	.skill-tag {
		display: inline-block;
		list-style: none;
		background: lightcoral;
		border-radius: 12px;
		padding: 5px 8px;
		font-size: 0.75rem;
		color: black;
		margin-right: 0.25rem;
		margin-bottom: 0.25rem;
	}
	svg {
		margin-bottom: 0.43rem;
	}
	a {
		font-weight: 500;
	}
	a:hover {
		color: pink;
	}
	#td-name-mobile {
		display: none;
	}
	@keyframes move-right {
		0% {
			transform: translate(0, 0);
		}
		100% {
			transform: translate(3px);
		}
	}
	@media only screen and (max-width: 675px) {
		#td-company,
		#link-td,
		#td-name {
			display: none;
		}
		#td-name-mobile {
			display: table-cell;
		}

		a:hover svg {
			animation: move-right 1s ease-in-out;
			animation-fill-mode: forwards;
		}
	}
</style>
