<script>
	// @ts-nocheck

	let nameintro = {
		'1': 'A ',
		'2': 'Self ',
		'3': 'Thought ',
		'4': 'Web ',
		'5': '&',
		'6': 'App',
		'7': 'Developer',
		'8': 'And',
		'9': 'A',
		'10': 'Tech',
		'11': 'Enthusiast',
		'12': 'From',
		'13': 'Palakkad',
		'14': 'Kerala'
	};
</script>

<div id="mainBdy">
	<h3 class="typing">I AM ANJITHA J.</h3>
	<div id="nameintro">
		{#each Object.keys(nameintro) as key}
			<span class="nameintro">{nameintro[key]} &nbsp;</span>
		{/each}
	</div>
</div>

<style>
	#mainBdy {
		width: 100vw;
		height: 90vh;
		background-image: url('https://ik.imagekit.io/0ta3q23cu/anjitha-portfolio/AnjBG.jpg?updatedAt=1691850034750');
		display: flex;
		flex-direction: column;
		justify-content: end;
		background-size: cover;
		background-position: 0vh;
		background-repeat: no-repeat;
		padding: 10px;
		-webkit-box-shadow: 0 10px 6px -6px #0011ff;
		-moz-box-shadow: 0 10px 6px -6px #0011ff;
		box-shadow: 0 10px 6px -6px #0011ff;
	}

	h3 {
		color: rgb(56, 111, 252);
		font-size: clamp(60px, 5vw, 90px);
		width: 17ch;
		border-right: 4px solid black;
		margin: 2rem auto;
		white-space: nowrap;
		overflow: hidden;
		text-align: center;
		padding-bottom: 5px;
		text-shadow: 0 0 160px #0011ff;
		animation: typing 2s steps(13, end), blink-caret 0.5s step-end infinite alternate;
	}

	#nameintro {
		color: rgb(255, 255, 255);
		text-align: center;
		font-family: 'Montserrat Medium';
		font-size: clamp(30px, 3vw, 60px);
		font-weight: bold;
		animation: scale 3s forwards cubic-bezier(0.5, 1, 0.89, 1);
	}
	span {
		display: inline-block;
		opacity: 0;
		filter: blur(4px);
	}

	@keyframes typing {
		from {
			width: 0;
		}
	}
	@keyframes blink-caret {
		50% {
			border-color: transparent;
		}
	}
	@keyframes fade-in {
		100% {
			opacity: 1;
			filter: blur(0);
		}
	}
	@keyframes scale {
		100% {
			transform: scale(1);
		}
	}

	span:nth-child(1) {
		animation: fade-in 0.8s 0.1s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(2) {
		animation: fade-in 0.8s 0.2s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(3) {
		animation: fade-in 0.8s 0.3s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(4) {
		animation: fade-in 0.8s 0.4s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(5) {
		animation: fade-in 0.8s 0.5s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(6) {
		animation: fade-in 0.8s 0.6s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(7) {
		animation: fade-in 0.8s 0.7s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(8) {
		animation: fade-in 0.8s 0.8s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(9) {
		animation: fade-in 0.8s 0.9s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(10) {
		animation: fade-in 0.8s 1s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(11) {
		animation: fade-in 0.8s 1.1s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(12) {
		animation: fade-in 0.8s 1.2s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(13) {
		animation: fade-in 0.8s 1.3s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}

	span:nth-child(14) {
		animation: fade-in 0.8s 1.4s forwards cubic-bezier(0.11, 0, 0.5, 0);
	}
</style>
