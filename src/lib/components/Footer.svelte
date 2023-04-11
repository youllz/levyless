<script>

</script>

<footer>
	

	
	<div class="body">
		<ul class="nav-links">
			<li><h3>Navigation</h3></li>
			<li><a href="/home">acceuil</a></li>
			<li><a href="/services">services</a></li>
			<li><a href="/about">a propos</a></li>
			<li><a href="/gallery">gallerie</a></li>
		</ul>
		<ul class="social">
			<li><h3>social</h3></li>
			<li>
			<a href="/">facebook</a>
			</li>
			<li>
				<a href="/">whatsapp</a>
			</li>
			<li>
			<a href="/">instagram</a>
			</li>
		</ul>
		<ul class="mail">
			<li>
				<h3>
					Obtenez des informations précieuses sur la stratégie, <br /> la culture et la marque directement
					dans votre boîte de réception
				</h3>
			</li>
			<li>
				<form action="/" method="POST">
					<input
						type="email"
						name="email"
						id="email"
						placeholder="Votre email"
						autocomplete="off"
					/>
					<button type="submit" title="envoyer">
						<span>
							<svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"
								><path
									fill="currentColor"
									d="M1.946 9.315c-.522-.174-.527-.455.01-.634l19.087-6.362c.529-.176.832.12.684.638l-5.454 19.086c-.15.529-.455.547-.679.045L12 14l6-8l-8 6l-8.054-2.685z"
								/></svg
							>
						</span>
					</button>
				</form>
			</li>
		</ul>
	</div>
	<div class="footer" >
    <h3>Copyright © 2023 LevyLess® | Abidjan |  CI </h3>
  </div>
</footer>

<style lang="scss">

  footer {
    padding: 3vw;
    margin-top: 10vw;
  }

	.body {
		// margin-top: 5rem;
		width: 100%;
		display: flex;
		justify-content: space-between;
		align-items: flex-start;
    flex-wrap: wrap;
		h3 {
			font-size: clamp(1.2rem, 2vw + .1rem, 18px);
			font-weight: bold;
		}
		a {
			color: var(--headline);
			opacity: 0.5;
			transition: opacity 0.3s ease;
			&:hover {
				opacity: 1;
			}
		}
	}
	.social {
		font-size: clamp(1rem, 4vw, 18px);
    display: flex;
    flex-direction: column;
    gap: 5px;
	}
	form {
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: center;

		input {
			width: clamp(100%, 50vw, 600px);
			height: 5rem;
			background-color: inherit;
			color: var(--main);
			border: none;
			padding: 0 1rem;
      font-size: clamp(1rem, 2vw , 18px);
      border-bottom: 1px solid var(--headline);

      &:focus {
        outline: none;
        border-bottom: 2px solid salmon;
      }
		}
		button {
			background-color: inherit;
			border: none;
			outline: none;
			color: var(--main);
			cursor: pointer;
      &:hover {
        opacity: 0.7;
      }
		}
	}
	.mail {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 3vw;

    h3 {
      font-size: clamp(1rem, 4vw, 18px);
    }


	}
  .footer {
    margin-top: 5vw;
    text-align: center;
  }

  .nav-links {
    display: flex;
    flex-direction: column;
    gap: 5px;
    font-size: clamp(1rem, 4vw, 18px);
  }
</style>