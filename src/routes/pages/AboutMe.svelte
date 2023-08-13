<div id="SecondBody">
	<div id="details">
		<div class="txt" id="AboutMe">
			<h1>About Me</h1>
			<p>
				I am Anjitha J, a passionate web Developer and tech enthusiast hailing from Palakkad,
				Kerala. Currently, I am pursuing my B. Tech in Electronics and Communication Engineering
				from Government Engineering College Thrissur. As a self-taught developer, I am always eager
				to stay updated with the latest technologies. I possess strong teamwork skills and excel in
				presentation and organizational abilities.
			</p>
		</div>
		<div class="txt" id="Education">
			<h1>Education</h1>
			<p>
				2020-Present : B. Tech in Electronics and Communication Engineering from Government
				Engineering College Thrissur. <br />
				2017-2019 : Higher Secondary Education from Jawahar Navodaya Vidyalaya, Palakkad. <br />
				2017: Secondary Education from Jawahar Navodaya Vidyalaya, Palakkad. <br />
			</p>
		</div>
		<div class="txt" id="Hobbies">
			<h1>My Hobbies</h1>
			<p>
				I have a strong passion for technology, especially laptops and mobile phones, as well as
				cars, bikes, and a wide range of topics like DIY projects, paleontology, cricket, human
				anatomy, psychology, films, and series. I stay updated through YouTube recommendations and
				run a WordPress website with a friend, where we discuss tech-related subjects and explore
				affiliate marketing as a passive income opportunity. Additionally, I co-own a tech YouTube
				channel. While I used to enjoy reading books, like most people, I now primarily rely on the
				internet for knowledge. I also have a deep love for music and enjoy listening to various
				genres.
			</p>
		</div>
		<div class="txt" id="Projects">
			<h1>My Projects</h1>
			<p>
				My primary focus is on creating apps and websites with user-friendly interfaces. I
				specialize in web development using Svelte, CSS, and Vanilla JavaScript. Occasionally, I
				also utilize React when the need arises. Moreover, I possess expertise in native app
				development using Flutter. I have completed multiple projects in various stacks, all of
				which are added to my GitHub repository. Additionally, I have a keen interest in expanding
				my expertise in web development and learning new technologies. I thoroughly enjoy content
				creation and have adept skills in handling WordPress.
			</p>
		</div>
		<div class="txt" id="Experience">
			<h1>My Experience</h1>
			<p>
				I have developed several impressive apps, web apps, and websites, though I sometimes wonder
				if they qualify as 'experience.' Besides, I manage a tech website with a substantial
				following and contribute to the Webteam for our college's IEEE Chapter. Additionally, I
				serve as the placement cell representative for the ECE 2020-2024 batch, utilizing my
				organizational skills effectively.
			</p>
		</div>
	</div>
</div>

<style>
	#SecondBody {
		display: flex;
		flex-direction: column;
	}

	@keyframes scale {
		100% {
			transform: scale(1);
		}
	}

	@keyframes fade-in {
		100% {
			opacity: 1;
			filter: blur(0);
		}
	}

	#details {
		color: white;
		width: 100vw;
		border-radius: 10px;
		padding: 20px;
		align-items: center;
		display: flex;
		flex-direction: column;
		justify-content: center;
		
	}
	.txt {
		background-color: rgb(17, 17, 17);
		padding: 20px;
		margin: 20px;
		border-radius: 50px;
		-webkit-box-shadow: 0 10px 6px -6px #0011ff;
		-moz-box-shadow: 0 10px 6px -6px #0011ff;
		box-shadow: 0 10px 6px -6px #0011ff;
		text-align: justify;
		word-wrap: break-word;
		margin: 20;
		width: clamp(350px, 50vw, 1000px);
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		font-size: 15px;
	}
	.txt:hover {
		animation: swiggle 0.5s forwards;
	}

	@keyframes swiggle {
		25% {
			transform: scale(0.9);
			background-color: rgb(17, 17, 17);
			-webkit-transform: rotateZ(2deg);
			-ms-transform: rotateZ(2deg);
			transform: rotateZ(2deg);
		}
		50% {
			background-color: rgb(17, 17, 17);
			-webkit-transform: rotateZ(-2deg);
			-ms-transform: rotateZ(-2deg);
			transform: rotateZ(-2deg);
			scale: 1.2;
		}
	}
	h1 {
		text-align: center;
		padding-bottom: 5px;
		font-size: 26px;
		color: #15d9f3;
	}
	p {
		text-align: justify;
		font-size: 22px;
		padding-left: 10px;
		padding-right: 10px;
	}
	@media screen and (max-width: 1000px){
		p {
		font-size: 15px;
	}
	}
</style>
