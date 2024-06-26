<script>
	export let name;
	export let bio;
	export let image;
	export let img_alt;
	export let link;
</script>

<a href={link} target="_blank" class="contrast">
	<div class="grid project">
		<div class="img-side">
			<img src={image} alt={img_alt} />
		</div>
		<div class="text-side">
			<p style="font-size: 1rem;">{name}</p>
			<p class="bio">{bio}</p>
		</div>
		<svg
			xmlns="http://www.w3.org/2000/svg"
			height="24px"
			viewBox="0 -960 960 960"
			width="24px"
			fill="currentColor"
			class="arrow"
			><path
				d="m216-160-56-56 464-464H360v-80h400v400h-80v-264L216-160Z"
			/></svg
		>
	</div>
</a>

<style lang="CSS">
	.arrow {
		grid-column: 8/8;
		width: 30px;
		height: 30px;
	}
	a {
		text-decoration: none !important;
		color: #c2c7d0;
	}
	.project:hover {
		background-color: rgba(61, 58, 58, 0.4);
		border-radius: 12px;
	}
	.project:hover .arrow {
		animation: move-top-right 1s ease-in-out;
		animation-fill-mode: forwards;
		color: #f08080;
	}
	.grid {
		display: grid;
		grid-template-columns: repeat(7, 1fr);
		padding: 10px;
	}
	img {
		object-fit: cover;
		width: 100px;
		height: 100px;
		border-radius: 6px;
		margin-top: 0.24rem;
	}
	.img-side {
		grid-column: 1/3;
	}
	.text-side {
		grid-column: 3/8;
	}
	.text-side > .bio {
		font-size: 0.7rem;
		line-height: 1rem;
	}

	@keyframes move-top-right {
		0% {
			transform: translate(0, 0);
		}
		100% {
			transform: translate(3px, -3px);
		}
	}
</style>
