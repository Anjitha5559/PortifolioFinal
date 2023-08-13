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
		<div class="circle deg-30">CSS</div>
		<div class="circle deg-60">JS</div>
		<div class="circle deg-90">React</div>
		<div class="circle deg-120">Flutter</div>
		<div class="circle deg-150">Firebase</div>
		<div class="circle deg-180">C</div>
		<div class="circle deg-210">C++</div>
		<div class="circle deg-240">Python</div>
		<div class="circle deg-270">MySQL</div>
		<div class="circle deg-300">Svelte</div>
		<div class="circle deg-330">Java</div>
	  </div>
</div>

<style>
	#skillheading {
		/* width: clamp(400px, 80vw, 800px); */
		margin-bottom: 1vh;
		border-radius: 10px;
		text-align: center;
	}

	.circle-wrapper {
		width: 500px;
		height: 500px;
		border-radius: 51%;
		background: rgb(0, 0, 0);
		position: relative;
		margin: auto;
		padding-bottom: 20px;
		margin-bottom: 200px;
		margin-top: 50px;
		font-size: 25px;
	}

	.circle {
		display: block;
		position: absolute;
		top: 50%;
		left: 40%;
		width: 150px;
		height:150px;
		margin: -0px;
		background: rgb(17, 17, 17);
		border-radius: 51%;
		text-align: center;
		line-height: 150px;
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
    transform: translate(270px);
  }
  .deg-30 {
    transform: rotate(30deg) translate(270px) rotate(-30deg);
  }
  .deg-60 {
    transform: rotate(60deg) translate(270px) rotate(-60deg);
  }
  .deg-90 {
    transform: rotate(90deg) translate(270px) rotate(-90deg);
  }
  .deg-120 {
    transform: rotate(120deg) translate(270px) rotate(-120deg);
  }
  .deg-150 {
    transform: rotate(150deg) translate(270px) rotate(-150deg);
  }
  .deg-180 {
    transform: rotate(180deg) translate(270px) rotate(-180deg);
  }
  .deg-210 {
    transform: rotate(210deg) translate(270px) rotate(-210deg);
  }
  .deg-240 {
    transform: rotate(240deg) translate(270px) rotate(-240deg);
  }
  .deg-270 {
    transform: rotate(270deg) translate(270px) rotate(-270deg);
  }
  .deg-300 {
    transform: rotate(300deg) translate(270px) rotate(-300deg);
  }
  .deg-330 {
    transform: rotate(330deg) translate(270px) rotate(-330deg);
  }
    

	@media screen and (max-width: 1300px) {
		.circle {
		width: 80px;
		height:80px;
		line-height: 80px;
		top: 50%;
		left: 33%;
	}
	.circle-wrapper {
		width: 300px;
		height: 300px;
		margin-bottom: 50px;
		margin-top: 50px;
		font-size: 10px;
	}

	@keyframes rotate {
		0%,
		75% {
			transform: rotateY(360deg);
		}
	}

	.deg-0 {
    transform: translate(140px);
  }
  .deg-30 {
    transform: rotate(30deg) translate(140px) rotate(-30deg);
  }
  .deg-60 {
    transform: rotate(60deg) translate(140px) rotate(-60deg);
  }
  .deg-90 {
    transform: rotate(90deg) translate(140px) rotate(-90deg);
  }
  .deg-120 {
    transform: rotate(120deg) translate(140px) rotate(-120deg);
  }
  .deg-150 {
    transform: rotate(150deg) translate(140px) rotate(-150deg);
  }
  .deg-180 {
    transform: rotate(180deg) translate(140px) rotate(-180deg);
  }
  .deg-210 {
    transform: rotate(210deg) translate(140px) rotate(-210deg);
  }
  .deg-240 {
    transform: rotate(240deg) translate(140px) rotate(-240deg);
  }
  .deg-270 {
    transform: rotate(270deg) translate(140px) rotate(-270deg);
  }
  .deg-300 {
    transform: rotate(300deg) translate(140px) rotate(-300deg);
  }
  .deg-330 {
    transform: rotate(330deg) translate(140px) rotate(-330deg);
  }

}

</style>
