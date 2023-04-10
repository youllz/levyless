<section>
	<div class="line-1">
		<!--  -->
		<article>
			<figure>
				<img
					src="https://images.unsplash.com/photo-1606216794074-735e91aa2c92?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1374&q=80"
					alt=""
				/>
			</figure>
			<div class="descript">
				<h4>MARIAGE DE CHECK</h4>
			</div>
		</article>
		<!--  -->
		<!--  -->
		<article>
			<figure>
				<img
					src="https://images.unsplash.com/photo-1606216794074-735e91aa2c92?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1374&q=80"
					alt=""
				/>
			</figure>
			<div class="descript">
				<h4>MARIAGE DE CHECK</h4>
			</div>
		</article>
		<!--  -->
	</div>
	<div class="line-2">
		<!--  -->
		<article>
			<figure>
				<img
					src="https://images.unsplash.com/photo-1606216794074-735e91aa2c92?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1374&q=80"
					alt=""
				/>
			</figure>
			<div class="descript">
				<h4>MARIAGE DE CHECK</h4>
			</div>
		</article>
		<!--  -->
		<!--  -->
		<article>
			<figure>
				<img
					src="https://images.unsplash.com/photo-1606216794074-735e91aa2c92?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1374&q=80"
					alt=""
				/>
			</figure>
			<div class="descript">
				<h4>MARIAGE DE CHECK</h4>
			</div>
		</article>
		<!--  -->
	</div>

	<div class="line-3">
		<article>
			<figure>
				<img
					src="https://images.unsplash.com/photo-1606216794074-735e91aa2c92?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1374&q=80"
					alt=""
				/>
			</figure>
			<div class="descript">
				<h4>MARIAGE DE CHECK</h4>
			</div>
		</article>
	</div>

	<div class="more">
		<a href="/"
			>VOIR PLUS DE PROJETS <span
				><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"
					><path
						fill="currentColor"
						d="m14 18l-1.4-1.45L16.15 13H4v-2h12.15L12.6 7.45L14 6l6 6l-6 6Z"
					/></svg
				></span
			></a
		>
	</div>
</section>

<div class="marquee-container">
	<div class="marquee">EXPERTISE - EXPERIENCE</div>
</div>

<style lang="scss">
	section {
		width: 100dvw;
		height: 100%;
		padding: 2vw;
		padding-top: 7vw;
		overflow: hidden;
	}

	article {
		width: clamp(300px, 30vw, 40rem);

		figure {
			width: 100%;
			height: 400px;
			overflow: hidden;
		}

		img {
			width: 100%;
			height: 100%;
			object-fit: cover;
			transition: all 0.3s;

			&:hover {
				margin-top: 20px;
				transform: scale(1.1);
			}
		}

		.descript {
			margin-top: 20px;
		}
	}

	.line-1 {
		width: 100%;
		display: flex;
		justify-content: space-around;
		// background-color: red;

		article:nth-child(2) {
			margin-top: 5vw;
			width: clamp(300px, 40vw, 60rem);
		}
	}

	.line-2 {
		display: flex;
		justify-content: space-between;
		margin-top: 10vw;

		article:nth-child(1) {
			margin-top: 5vw;
			width: clamp(300px, 40vw, 60rem);
		}
	}

	.line-3 {
		margin-top: 10vw;
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: center;

		article {
			width: clamp(500px, 50vw, 60rem);
		}
	}

	.more {
		margin-top: 5vw;
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: center;

		svg {
			transition: all 0.3s;
		}

		a {
			display: flex;
			align-items: center;
			position: relative;
			// overflow: hidden;

			&::before {
				content: '';
				display: block;
				position: absolute;
				width: 100%;
				height: 2px;
				background-color: #fff;
				bottom: -1px;
				transform: scaleX(0);
				transition: all 0.3s;
				transform-origin: left;
			}

			&:hover {
				svg {
					transform: translateX(15px);
				}
			}

			&:hover::before {
				transform: scaleX(1);
				transform-origin: left;
			}
		}
	}
	.marquee-container {
		width: 100dvw;
		overflow: hidden;

		margin-top: 10vw;

		.marquee {
			width: 100%;
			display: flex;
			align-items: center;
			white-space: nowrap;
			font-size: 8vw;
			animation: marquee 10s infinite linear;
		}
	}

	.marquee::after {
		content: '- EXPERTISE - EXPERIENCE -';
	}

  @keyframes marquee {
    0% {
      transform: translateX(0);
    }
    
    100% {
      transform: translateX(-50%);

    }
  }
</style>
