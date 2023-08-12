<script>
	let contactdetails = [
		{
			name: 'Email',
			link: 'mailto:anjithajsobha@gail.com',
			color: '#D44638'
		},
		{
			name: 'Phone',
			link: 'tel:9447400037',
			color: '#AAB54A'
		},
		{
			name: 'Whatsapp',
			link: 'wa.me/9447400037',
			color: '#3AB54A'
		},
		{
			name: 'LinkedIn',
			link: 'https://www.linkedin.com/in/anjitha-j/',
			color: '#0077B5'
		},
		{
			name: 'Github',
			link: 'https://github.com/Anjitha5559',
			color: '#333333'
		}
	];
	let heading = 'Connect^with^me';
</script>

<div id="Contact_box">
	<h3 class="rotate">
		{#each heading as letter, i}
			{#if letter == '^'}
				<span> &nbsp;</span>
			{:else}
				<span style="animation-delay: {i * 0.1}s">{letter}</span>
			{/if}
		{/each}
	</h3>

	<div id="ContactMe">
		{#each contactdetails as contact}
			<div class="contact_btn" style="background-color: {contact.color};">
				<a href={contact.link} target="_blank" rel="noopener noreferrer">
					{contact.name}
				</a>
			</div>
		{/each}
	</div>
</div>

<style>
	#Contact_box {
		width: clamp(400px, 80vw, 800px);
		background-color: black;
		margin: 3vw;
		padding: 1vw;
		border-radius: 10px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		-webkit-box-shadow: 0 10px 6px -6px #0011ff;
		-moz-box-shadow: 0 10px 6px -6px #0011ff;
		box-shadow: 0 10px 6px -6px #0011ff;
	}

	#ContactMe {
		width: 80%;
		display: flex;
		flex-direction: row;
		justify-content: space-evenly;
		align-items: center;
		flex-wrap: wrap;
	}
	a {
		text-decoration: none;
		color: #ffffff;
	}

	.contact_btn {
		font-weight: bolder;
		text-align: center;
		width: 100px;
		border-radius: 10px;
		padding: 10px;
		margin: 10px;
		text-align: center;
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
</style>
