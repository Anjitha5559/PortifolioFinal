<script>
	const year = {
		2001: {
			year: 2001,
			data: 'Born to Jayamani C and Sobhana D on 9 july 2001'
		},
		2002: {
			year: 2002,
			data: 'went to Delhi, and lived a life I will never forget'
		},
		2003: {
			year: 2003,
			data: 'Opened my mouth to speak, and have never shut up since'
		},
		2005: {
			year: 2005,
			data: 'My first School, Pooja Baal Niketan, was a place I loved'
		},
		2006: {
			year: 2006,
			data: ' I carried 5KG of rice in 1 Hand, but nobody believes me even now '
		},
		2007: {
			year: 2007,
			data: 'Had to start sharing my mother and father, my brother was cute though'
		},
		2008: {
			year: 2008,
			data: 'Came back to Kerala, and started my life here'
		},
		2009: {
			year: 2009,
			data: 'Lost my Dad, I still love him, and I still Miss him.'
		},
		2010: {
			year: 2010,
			data: 'Got my rabbit teeths'
		},
		2011: {
			year: 2011,
			data: ' Last of My streak of First price in Geetha Parayanam '
		},
		2012: {
			year: 2012,
			data: "Got into Navodya Vidyalaya, Palakkad. 'Come to learn, Go to serve.'"
		},
		2013: {
			year: 2013,
			data: ' my intrest in Computers started '
		},
		2014: {
			year: 2014,
			data: 'Became class topper after a while'
		},
		2015: {
			year: 2015,
			data: 'Went to Rajasthan, for a year. It gave me life experiences and outlook I will never forget'
		},
		2016: {
			year: 2016,
			data: "Got 10CGPA in X. Turns out 10th doens'nt decdide my life "
		},
		2017: {
			year: 2017,
			data: 'became the school captain. I think I was a good one'
		},
		2019: {
			year: 2019,
			data: 'turns out 12th wasnt the life decider either, and took part in Aswamedham Show'
		},
		2020: {
			year: 2020,
			data: ' Biggest decisitons in my life were taken, from Brilliant Pala, And Got into GEC Thrissur. new life, new ambitions'
		},
		2021: {
			year: 2021,
			data: 'Started learning Coding, and I Loved it, and loving it ever since. Also started our own Website and youtube channel'
		},
		2022: {
			year: 2022,
			data: 'Started winning Hacathons, maybe this is my thing. I hope so'
		},
		2023: {
			year: 2023,
			data: 'Became IEEE GEC Thrissur Web master, Probably will kickstart my career too.'
		},
		2024: {
			year: 2024,
			data: 'I hope I will be a good Engineer, and a good person'
		}
	};
</script>

<div id="bdy">
	<div id="myTime">
		<div class="timeline">
			{#each Object.values(year) as y, i}
				<div class="container {i % 2 === 0 ? 'right' : 'left'}">
					<div class="content">
						<h2 class="hyear">{y.year}</h2>
						<p>{y.data}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<style>
	#myTime {
		width: 90vw;
		height: 70vh;
	}

	* {
		box-sizing: border-box;
	}
	#bdy {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-between;
		padding: 15px;
		width: clamp(300px, 90vw, 1200px);
	}
	/* Set a background color */
	#myTime {
		width: 100%;
		background-color: rgb(22, 22, 22);
		padding: 10px;
		border-radius: 10px;
		-webkit-box-shadow: 0 10px 6px -6px #0011ff;
		-moz-box-shadow: 0 10px 6px -6px #0011ff;
		box-shadow: 0 10px 6px -6px #0011ff;
		height: 70vh;
		overflow: scroll;
		scrollbar-width: none;
		border-radius: 50px;
	}

	/* The actual timeline (the vertical ruler) */
	.timeline {
		position: relative;
		max-width: 1200px;
		margin: 0 auto;
	}

	/* The actual timeline (the vertical ruler) */
	.timeline::after {
		content: '';
		position: absolute;
		width: 6px;
		background-color: white;
		top: 0;
		bottom: 0;
		left: 50%;
		margin-left: -3px;
	}

	/* Container around content */
	.container {
		padding: 10px 40px;
		position: relative;
		background-color: inherit;
		width: 50%;
	}

	/* The circles on the timeline */
	.container::after {
		content: '';
		position: absolute;
		width: 25px;
		height: 25px;
		right: -17px;
		background-color: white;
		border: 4px solid #ff9f55;
		top: 15px;
		border-radius: 50%;
		z-index: 1;
	}

	/* Place the container to the left */
	.left {
		left: 0;
	}

	/* Place the container to the right */
	.right {
		left: 50%;
	}

	/* Add arrows to the left container (pointing right) */
	.left::before {
		content: ' ';
		height: 0;
		position: absolute;
		top: 22px;
		width: 0;
		z-index: 1;
		right: 30px;
		border: medium solid white;
		border-width: 10px 0 10px 10px;
		border-color: transparent transparent transparent white;
	}

	/* Add arrows to the right container (pointing left) */
	.right::before {
		content: ' ';
		height: 0;
		position: absolute;
		top: 22px;
		width: 0;
		z-index: 1;
		left: 30px;
		border: medium solid white;
		border-width: 10px 10px 10px 0;
		border-color: transparent white transparent transparent;
	}

	/* Fix the circle for containers on the right side */
	.right::after {
		left: -16px;
	}

	/* The actual content */
	.content {
		padding: 10px 10px;
		background-color: rgb(255, 237, 237);
		position: relative;
		border-radius: 6px;
		font-weight: bold;
	}
	.hyear {
		font-size: 2rem;
		font-weight: bolder;
		color: rgb(199, 39, 231);
		text-align: center;
	}
</style>
