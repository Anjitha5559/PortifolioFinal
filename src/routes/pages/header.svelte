
<div id="header">
	<div class="headitem">
		<!-- <img id="anjimg" src={Anjitha} alt="ANjitha" width="100px" height="100px" /> -->
	</div>
	<div id="heading" class="headitem">
		<div class="waviy">
			<span style="--i:1">M</span>
			<span style="--i:2">Y</span>
			<span style="--i:3" />
			<span style="--i:4">P</span>
			<span style="--i:5">O</span>
			<span style="--i:6">R</span>
			<span style="--i:7">T</span>
			<span style="--i:8">I</span>
			<span style="--i:9">F</span>
			<span style="--i:10">O</span>
			<span style="--i:11">L</span>
			<span style="--i:12">I</span>
			<span style="--i:13">O</span>
		</div>
	</div>
	<div id="menu" class="headitem">
		<div class="menubaby"><a href="#SecondBody">About Me</a></div>
		<div class="menubaby"><a href="#Contact_box">Projects</a></div>
		<div class="menubaby"><a href="#ContactHeading">Contact Me</a></div>
	</div>
</div>

<style>
	#header {
		font-weight: bolder;
		width: 100vw;
		height: 10vh;
		background-color: rgb(22, 22, 22);
		display: flex;
		flex-direction: row;
		justify-content: space-evenly;
		align-items: center;
		padding: 10px;
		box-shadow: 0px 0px 10px 0px white;
		/* flex-wrap: wrap; */
		
	}
	.headitem {
		width: 25%;
		/* width: 100%; */
	}

	.waviy {
		font-weight: bolder;
		position: relative;
		-webkit-box-reflect: below -20px linear-gradient(transparent, rgba(0, 0, 0, 0.2));
		font-size: clamp(2rem, 4vw, 3rem);
	}
	.waviy span {
		font-weight: bolder;
		font-family: "Poppins", sans-serif;
		position: relative;
		display: inline-block;
		color: rgb(0, 4, 255);
		text-transform: uppercase;
		animation: waviy 1s infinite;
		animation-delay: calc(0.1s * var(--i));

	}
	@keyframes waviy {
		0%,
		40%,
		100% {
			transform: translateY(0);
		}
		20% {
			transform: translateY(-20px);
		}
	}

	#heading {
		justify-content: center;
		align-items: center;
		text-align: center;
		font-weight: bolder;
		width: 100vw;
	}
	#menu {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
		color: white;
	}
	.menubaby {
		padding: clamp(2px, 5px, 10px);
		font-size: clamp(4px, 10px, 15px);

	}
	a {
		text-decoration: none;
		color: #ffffff;
	}
	@media screen and (max-width: 1000px){
		#header{
			flex-wrap: wrap;
		}
		.headitem {
		width: 50%;
	}
	}
</style>
