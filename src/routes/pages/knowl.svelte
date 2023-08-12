<script>
	let heading = 'My^Skills';
	let skills = [
		'html',
		'css',
		'js',
		'react',
		'flutter',
		'firebase',
		'c',
		'c++',
		'wordpress',
		'python',
		'mysql',
		'bootstrap',
		'svelte',
		'java',
		'8051',
		'arm'
	];
</script>

<div id="skillheading">
	<h3 class="rotate">
		{#each heading as letter, i}
			{#if letter == '^'}
				<span> &nbsp;</span>
			{:else}
				<span style="animation-delay: {i * 0.1}s">{letter}</span>
			{/if}
		{/each}
	</h3>

	<div class="circle-wrapper">
		<div class="circle deg-0">HTML</div>
		<div class="circle deg-22">CSS</div>
		<div class="circle deg-45">JS</div>
		<div class="circle deg-67">React</div>
		<div class="circle deg-90">Flutter</div>
		<div class="circle deg-112">Firebase</div>
		<div class="circle deg-135">C</div>
		<div class="circle deg-157">C++</div>
		<div class="circle deg-180">WordPress</div>
		<div class="circle deg-202">Python</div>
		<div class="circle deg-225">MySQL</div>
		<div class="circle deg-247">Bootstrap</div>
		<div class="circle deg-270">Svelte</div>
		<div class="circle deg-292">Java</div>
		<div class="circle deg-315">8051</div>
		<div class="circle deg-337">ARM</div>
	</div>
</div>

<style>
	#skillheading {
		width: clamp(400px, 80vw, 800px);
		margin: 2vh;
		padding: 2vh;
		border-radius: 10px;
		text-align: center;
	}

	.circle-wrapper {
		width: 90%;
		height: 700px;
		border-radius: 51%;
		position: relative;
		margin: auto;
		padding-bottom: 20px;
	}

	.circle {
		display: block;
		position: absolute;
		top: 40%;
		left: 40%;
		width: 100px;
		height: 100px;
		margin: -0px;
		background: rgb(17, 17, 17);
		border-radius: 51%;
		text-align: center;
		line-height: 100px;
		align-items: center;
		box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
		color: white;
		-webkit-box-shadow: 0 10px 6px -6px #0011ff;
		-moz-box-shadow: 0 10px 6px -6px #0011ff;
		box-shadow: 0 10px 6px -6px #0011ff;
		font-weight: bolder;
	}
	.circle:hover {
		-webkit-animation: hoverEffect 4s;
		animation: hoverEffect 4s;
		background-color: rgb(17, 17, 17);
		-webkit-transform: scale(2.1);
		-ms-transform: scale(2.1);
		transform: scale(2.1);
		transition: 3s ease;
	}

	.rotate span {
		font-size: clamp(1.5rem, 3vw, 3rem);
		color: #f8f8f8;
		display: inline-flex;
		animation: rotate 2s infinite;
	}
	@keyframes rotate {
		0%,
		75% {
			transform: rotateY(360deg);
		}
	}

	.deg-0 {
		transform: translate(251px);
	}
	.deg-22 {
		transform: rotate(23deg) translate(251px) rotate(-23deg);
	}

	.deg-45 {
		transform: rotate(46deg) translate(251px) rotate(-46deg);
	}
	.deg-67 {
		transform: rotate(68deg) translate(251px) rotate(-68deg);
	}
	.deg-90 {
		transform: rotate(91deg) translate(251px) rotate(-91deg);
	}
	.deg-112 {
		transform: rotate(113deg) translate(251px) rotate(-113deg);
	}
	.deg-135 {
		transform: rotate(136deg) translate(251px) rotate(-136deg);
	}
	.deg-157 {
		transform: rotate(158deg) translate(251px) rotate(-158deg);
	}
	.deg-180 {
		transform: rotate(181deg) translate(251px) rotate(-181deg);
	}
	.deg-202 {
		transform: rotate(203deg) translate(251px) rotate(-203deg);
	}
	.deg-225 {
		transform: rotate(226deg) translate(251px) rotate(-226deg);
	}
	.deg-247 {
		transform: rotate(248deg) translate(251px) rotate(-248deg);
	}

	.deg-270 {
		transform: rotate(271deg) translate(251px) rotate(-271deg);
	}
	.deg-292 {
		transform: rotate(293deg) translate(251px) rotate(-293deg);
	}
	.deg-315 {
		transform: rotate(316deg) translate(251px) rotate(-316deg);
	}
	.deg-337 {
		transform: rotate(338deg) translate(251px) rotate(-338deg);
	}
</style>
