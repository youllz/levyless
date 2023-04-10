<section>
  <div class="text">
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> Cupiditate consectetur illum id sint iure aliquid, ipsum quas nemo at, iusto dicta, deleniti deserunt delectus iste nam consequatur incidunt. Nobis, expedita.
    </p>
    <br>
    <br>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. In, quia quae necessitatibus, quod cumque eos inventore, tempora esse omnis numquam ipsam. Atque ex deleniti laboriosam id iste accusantium ad cum.
    </p>



    <div class="more">
      <a href="/"
        >NOTRE EQUIPE <span
          ><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"
            ><path
              fill="currentColor"
              d="m14 18l-1.4-1.45L16.15 13H4v-2h12.15L12.6 7.45L14 6l6 6l-6 6Z"
            /></svg
          ></span
        ></a
      >
    </div>
  </div>
  <div class="img">
    <img src="https://images.unsplash.com/photo-1610851467843-fe4a65aea9c0?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NDB8fGFmcmljYW4lMjBmb29kfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60" alt="">
  </div>
</section>

<style lang="scss"> 
  section {
    
    width: 100dvw;
    height: 100%;
    padding: 5vw;
    display: flex;
    gap: 30px;

    margin-top: 5vw;
    flex-direction: column;
    overflow: hidden;

  }


  .text {
    // max-width: 300px;
    order: 0;
  }

  .img {
    width: clamp(500px, 50vw, 60rem);
    height: clamp(300px, 30vw, 40rem);
    
    order: 1;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
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
</style>